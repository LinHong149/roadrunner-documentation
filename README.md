# Roadrunner Documentation

## Resources
- Road Runner Docs: https://rr.brott.dev/docs/v1-0/installation/

## Setup
1. Open `Teamcode build.gradle` and add
```
repositories {
    maven {
        url = 'https://maven.brott.dev/'
    }
}

dependencies {
    implementation project(':FtcRobotController')
    annotationProcessor files('lib/OpModeAnnotationProcessor.jar')

    implementation "com.acmerobotics.roadrunner:ftc:0.1.13"
    implementation "com.acmerobotics.roadrunner:core:1.0.0-beta8"
    implementation "com.acmerobotics.roadrunner:actions:1.0.0-beta8"
    implementation "com.acmerobotics.dashboard:dashboard:0.4.14"
}
```
2. Gradle sync
