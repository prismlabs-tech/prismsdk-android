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
    maven("https://maven.pkg.github.com/prismlabs-tech/prismsdk-android")
}
```

This will tell Gradle where to look for the PrismSDK.
