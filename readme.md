# GStreamer 1.0 example "tutorial 5" for Android Studio with Gradle

Here is working tutorial-5 example. Code originally came from [Sebastian Dröge (slomo) blog](https://coaxion.net).
To run this code on Android Studio, you have to make Gradle compile NDK code using .mk files
originally made for Eclipse.

Gradle code is made mainly thanks to [Gaku Ueada's blog post](http://blog.gaku.net/ndk/). For some
more details look at `app/build.gradle`.

## How to

1. Open project with Android Studio (tested with 1.0 version)
2. Edit `local.properties` - set SDK and NDK paths
3. Download GStreamer Android library from [freedesktop page](http://gstreamer.freedesktop.org/data/pkg/android/).
 I was using [1.4.4 version from 08-Nov-2014 10:03](http://gstreamer.freedesktop.org/data/pkg/android/1.4.4/)
 (gstreamer-1.0-android-arm-release-1.4.4.tar.bz2). Extract everything somewhere.
4. Edit `src/main/jni/Android.mk` file and set `GSTREAMER_ROOT_ANDROID` to the path
where your extracted Gstreamer library (step 3).
5. Run
