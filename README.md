# opencv-android

An easy way to integrate OpenCV into your Android project via Gradle.

**No NDK dependency needed** - just include this library and you are good to go.

## Usage

Include one the dependencies in your module's build.gradle file:

https://mvnrepository.com/artifact/com.quickbirdstudios/opencv

```groovy
dependencies {
    implementation 'com.quickbirdstudios:opencv:4.1.0'
}
```

Check https://mvnrepository.com/artifact/com.quickbirdstudios/opencv for available version

A version suffix `-contrib` indicates "with contribution packages".

Don't forget to also initialize OpenCV with a statement like this e.g. in your Application class:

```java
if (OpenCVLoader.initDebug()) {
    Log.d("OpenCv", "OpenCV loaded");
} else {
    Log.e("OpenCv", "Unable to load OpenCV");
}
```
