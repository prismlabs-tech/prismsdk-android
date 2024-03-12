[![Platforms](https://img.shields.io/badge/Platforms-Android-yellowgreen?style=flat-square)](https://img.shields.io/badge/Platforms-macOS_iOS_tvOS_watchOS_vision_OS_Linux_Windows_Android-Green?style=flat-square)

# PrismSDK

This SDK enables the users to integrate an existing application with the PrismLabs’ body mapping service. While using your phone’s front-facing camera, you can guide users through a simple and intuitive body mapping process.

Additionally, the `PrismSDK` communicates with the Prism-hosted API on your behalf, allowing you to create new users, submit scan data capture, and fetch results. 

Finally, Prism’s Pipeline transforms captured images into precise body models and delivers valuable insights about your body’s metrics.

## Prerequisites

- Android Studio
- Android 9 or Later

## Installation

### Gradle Instalation

To install the latest version of the package, simple add a new `implementation` entry to you `build.gradle` file. 

```kotlin
dependencies {
    // ...
    implementation("tech.prismlabs:prismsdk:0.0.3")
}
```

In order to install packages from GitHub you need to specify the repository 
```kotlin
repositories {
    //...
    maven {
         url = uri("https://maven.pkg.github.com/prismlabs-tech/prismsdk-android")
        credentials {
            username = "<github_username>"
            password = "<pat_token>"
        }
    }
}
```

Note: You can use environment variables to set the username and password for the maven credentials.

This will tell Gradle where to look for the PrismSDK.

In order for Gradle to be able to access the Github Maven Repository, you have to supply it with a username and personal access token with the permissions `read:packages`. 
This does not require access to this repo, its simply to authenticate with the GitHub API. This means a dummy github account, or a scoped access token strickly for package fetching will suffice.
