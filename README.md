# Build Environment Android
Light weight build environment for Android projects.

It includes:
- OpenJDK 8
- Android SDK
- Platform Tools
- Build Tools
- Android Support Library
- Google Play Services

## Build image
```
$ docker build -t musichin/build-environment-android .
```

## Run docker
```
$ docker run -it musichin/build-environment-android /bin/bash
```

## Build Android project
```
$ docker run -v $PWD:/project -it musichin/build-environment-android /bin/bash gradlew assembleRelease
```
