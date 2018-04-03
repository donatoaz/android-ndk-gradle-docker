# Android NDK Gradle
[![/android-ndk-gradle](http://dockeri.co/image/donatoaz/android-ndk-gradle-docker)](https://hub.docker.com/r/donatoaz/android-ndk-gradle-docker/)

## Included
* OpenJDK 8
* Git
* Gradle
  
  * **latest**: 3.3 (I know this sounds stupid, but I didn't know how to change on docker hub
  * **v2**: 4.5.1
* Android NDK r13b
* Android SDK (android-24,android-25)
* Android Build-tools (24.0.2,24.0.3,25.0.2,27.0.3)
* Android System Images(sys-img-armeabi-v7a-android-24,sys-img-armeabi-v7a-android-25)
* Android Support Libraries
* Google Play Services

## Build image

```bash
docker build -t donatoaz/android-ndk-gradle-docker:v2 .
```

### Usage

```bash
docker pull donatoaz/android-ndk-gradle-docker:v2
```

Change directory to your project directory, then run:

```bash
docker run -ti --volume=$(pwd):/opt/workspace --user `id -u` --workdir=/opt/workspace --rm donatoaz/android-ndk-gradle-docker /bin/bash
```
