# Comparing `tmp/peek-field-app-3.3.3.tar.gz` & `tmp/peek-field-app-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-app-3.3.3.tar", last modified: Mon Nov 14 05:36:02 2022, max compression
+gzip compressed data, was "peek-field-app-3.4.0.tar", last modified: Wed Apr 12 11:04:45 2023, max compression
```

## Comparing `peek-field-app-3.3.3.tar` & `peek-field-app-3.4.0.tar`

### file list

```diff
@@ -1,258 +1,260 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.827246 peek-field-app-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      360 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1038 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.816245 peek-field-app-3.3.3/peek_field_app/
--rw-r--r--   0 root         (0) root         (0)      487 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/.browserslistrc
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/.gitignore
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1082 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/README.md
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/
--rw-r--r--   0 root         (0) root         (0)     1589 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/
--rw-r--r--   0 root         (0) root         (0)       26 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/.npmignore
--rw-r--r--   0 root         (0) root         (0)     1523 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/build.gradle
--rw-r--r--   0 root         (0) root         (0)      746 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/capacitor.build.gradle
--rw-r--r--   0 root         (0) root         (0)      751 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/proguard-rules.pro
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.812245 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.812245 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.812245 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.812245 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/
--rw-r--r--   0 root         (0) root         (0)      757 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/
--rw-r--r--   0 root         (0) root         (0)     2762 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/assets/
--rw-r--r--   0 root         (0) root         (0)      207 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/assets/capacitor.config.json
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/assets/capacitor.plugins.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/com/synerty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/com/synerty/peek/
--rw-r--r--   0 root         (0) root         (0)      534 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.817246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable/
--rw-r--r--   0 root         (0) root         (0)     5589 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0 root         (0) root         (0)     4040 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-hdpi/
--rw-r--r--   0 root         (0) root         (0)     7705 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-mdpi/
--rw-r--r--   0 root         (0) root         (0)     4040 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     9251 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)    13984 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)    17683 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-hdpi/
--rw-r--r--   0 root         (0) root         (0)     7934 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-mdpi/
--rw-r--r--   0 root         (0) root         (0)     4096 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     9875 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)    13346 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)    17489 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-v24/
--rw-r--r--   0 root         (0) root         (0)     1897 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/layout/
--rw-r--r--   0 root         (0) root         (0)      538 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/layout/activity_main.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.818246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/
--rw-r--r--   0 root         (0) root         (0)      265 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
--rw-r--r--   0 root         (0) root         (0)      265 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.819245 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/
--rw-r--r--   0 root         (0) root         (0)     2786 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     3450 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     4341 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.819245 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/
--rw-r--r--   0 root         (0) root         (0)     1869 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     2110 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     2725 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.819245 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/
--rw-r--r--   0 root         (0) root         (0)     3981 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     5036 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)     6593 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.819245 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/
--rw-r--r--   0 root         (0) root         (0)     6644 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)     9793 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)    10455 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.819245 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/
--rw-r--r--   0 root         (0) root         (0)     9441 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
--rw-r--r--   0 root         (0) root         (0)    15529 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png
--rw-r--r--   0 root         (0) root         (0)    15916 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/values/
--rw-r--r--   0 root         (0) root         (0)      120 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/values/ic_launcher_background.xml
--rw-r--r--   0 root         (0) root         (0)      280 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/values/strings.xml
--rw-r--r--   0 root         (0) root         (0)      816 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/values/styles.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/xml/
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/xml/config.xml
--rw-r--r--   0 root         (0) root         (0)      211 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/xml/file_paths.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.813246 peek-field-app-3.3.3/peek_field_app/android/app/src/test/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.814246 peek-field-app-3.3.3/peek_field_app/android/app/src/test/java/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.814246 peek-field-app-3.3.3/peek_field_app/android/app/src/test/java/com/getcapacitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/
--rw-r--r--   0 root         (0) root         (0)      391 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/ExampleUnitTest.java
--rw-r--r--   0 root         (0) root         (0)      622 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/build.gradle
--rw-r--r--   0 root         (0) root         (0)     1199 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/capacitor.settings.gradle
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.814246 peek-field-app-3.3.3/peek_field_app/android/gradle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/android/gradle/wrapper/
--rw-r--r--   0 root         (0) root         (0)    55616 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 root         (0) root         (0)      233 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0 root         (0) root         (0)     1072 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/gradle.properties
--rwxr-xr-x   0 root         (0) root         (0)     5856 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/gradlew
--rw-r--r--   0 root         (0) root         (0)     2842 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/gradlew.bat
--rw-r--r--   0 root         (0) root         (0)      208 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/settings.gradle
--rw-r--r--   0 root         (0) root         (0)      562 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/android/variables.gradle
--rw-r--r--   0 root         (0) root         (0)     7284 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/angular.json
--rw-r--r--   0 root         (0) root         (0)      355 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/capacitor.config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/e2e/
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/e2e/app.e2e-spec.ts
--rw-r--r--   0 root         (0) root         (0)      227 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/e2e/app.po.ts
--rw-r--r--   0 root         (0) root         (0)      367 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/e2e/tsconfig.e2e.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/ios/
--rw-r--r--   0 root         (0) root         (0)      260 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/ios/App/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.820246 peek-field-app-3.3.3/peek_field_app/ios/App/App/
--rw-r--r--   0 root         (0) root         (0)     3829 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/AppDelegate.swift
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.822245 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 root         (0) root         (0)      774 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png
--rw-r--r--   0 root         (0) root         (0)     2095 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png
--rw-r--r--   0 root         (0) root         (0)     2095 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png
--rw-r--r--   0 root         (0) root         (0)     3346 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png
--rw-r--r--   0 root         (0) root         (0)     1376 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png
--rw-r--r--   0 root         (0) root         (0)     3116 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png
--rw-r--r--   0 root         (0) root         (0)     3116 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png
--rw-r--r--   0 root         (0) root         (0)     5450 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png
--rw-r--r--   0 root         (0) root         (0)     2095 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png
--rw-r--r--   0 root         (0) root         (0)     4812 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png
--rw-r--r--   0 root         (0) root         (0)     4812 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png
--rw-r--r--   0 root         (0) root         (0)     7945 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png
--rw-r--r--   0 root         (0) root         (0)   110522 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png
--rw-r--r--   0 root         (0) root         (0)     8284 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png
--rw-r--r--   0 root         (0) root         (0)    14116 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png
--rw-r--r--   0 root         (0) root         (0)     4530 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png
--rw-r--r--   0 root         (0) root         (0)    10502 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png
--rw-r--r--   0 root         (0) root         (0)    11606 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png
--rw-r--r--   0 root         (0) root         (0)     2889 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 root         (0) root         (0)       72 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Contents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.822245 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/
--rw-r--r--   0 root         (0) root         (0)      485 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/Contents.json
--rw-r--r--   0 root         (0) root         (0)    41273 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png
--rw-r--r--   0 root         (0) root         (0)    41273 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png
--rw-r--r--   0 root         (0) root         (0)    41273 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.823245 peek-field-app-3.3.3/peek_field_app/ios/App/App/Base.lproj/
--rw-r--r--   0 root         (0) root         (0)     1994 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0 root         (0) root         (0)     1019 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Base.lproj/Main.storyboard
--rw-r--r--   0 root         (0) root         (0)     2809 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/Info.plist
--rw-r--r--   0 root         (0) root         (0)      289 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/capacitor.config.json
--rw-r--r--   0 root         (0) root         (0)      385 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App/config.xml
--rw-r--r--   0 root         (0) root         (0)     2418 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App copy-Info.plist
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/
--rw-r--r--   0 root         (0) root         (0)    16799 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/project.pbxproj
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/
--rw-r--r--   0 root         (0) root         (0)      148 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.814246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/xcshareddata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 root         (0) root         (0)     2804 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcworkspace/
--rw-r--r--   0 root         (0) root         (0)      221 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.821246 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcworkspace/xcshareddata/
--rw-r--r--   0 root         (0) root         (0)      238 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/App.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0 root         (0) root         (0)     1131 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/ios/App/Podfile
--rw-r--r--   0 root         (0) root         (0)     1341 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/karma.conf.js
--rw-r--r--   0 root         (0) root         (0)   674119 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     2938 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app/package.json
--rw-r--r--   0 root         (0) root         (0)      868 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/protractor.conf.js
--rw-r--r--   0 root         (0) root         (0)      279 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/proxy.conf.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.823245 peek-field-app-3.3.3/peek_field_app/scripts/
--rwxr-xr-x   0 root         (0) root         (0)    14824 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/scripts/build_capacitor_app.sh
--rw-r--r--   0 root         (0) root         (0)      734 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/scripts/exportOptionsPlist.plist.template
--rwxr-xr-x   0 root         (0) root         (0)     2601 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/scripts/prepare_capacitor_ios_app.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.823245 peek-field-app-3.3.3/peek_field_app/src/
--rw-r--r--   0 root         (0) root         (0)     1129 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/_components.scss
--rw-r--r--   0 root         (0) root         (0)     1343 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/_variables.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/
--rw-r--r--   0 root         (0) root         (0)     2499 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/app.module.ts
--rw-r--r--   0 root         (0) root         (0)     1110 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/app.routes.ts
--rw-r--r--   0 root         (0) root         (0)      834 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/app.services.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/core/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/core/components/app/
--rw-r--r--   0 root         (0) root         (0)      471 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/app/app.component.html
--rw-r--r--   0 root         (0) root         (0)      181 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/app/app.component.scss
--rw-r--r--   0 root         (0) root         (0)     2257 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/app/app.component.ts
--rw-r--r--   0 root         (0) root         (0)      859 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/components.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/
--rw-r--r--   0 root         (0) root         (0)     2207 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.html
--rw-r--r--   0 root         (0) root         (0)     1325 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.scss
--rw-r--r--   0 root         (0) root         (0)     2063 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.ts
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/index.ts
--rw-r--r--   0 root         (0) root         (0)       37 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/index.ts
--rw-r--r--   0 root         (0) root         (0)      861 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      499 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/status.component.scss
--rw-r--r--   0 root         (0) root         (0)     1585 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/status.component.ts
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/core/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.824246 peek-field-app-3.3.3/peek_field_app/src/app/pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.825245 peek-field-app-3.3.3/peek_field_app/src/app/pages/config/
--rw-r--r--   0 root         (0) root         (0)      946 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/config/config.page.html
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/config/config.page.scss
--rw-r--r--   0 root         (0) root         (0)      787 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/config/config.page.ts
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/config/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.825245 peek-field-app-3.3.3/peek_field_app/src/app/pages/home/
--rw-r--r--   0 root         (0) root         (0)     1109 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/home/home.page.html
--rw-r--r--   0 root         (0) root         (0)     1874 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/home/home.page.scss
--rw-r--r--   0 root         (0) root         (0)     1748 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/home/home.page.ts
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/home/index.ts
--rw-r--r--   0 root         (0) root         (0)      126 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/index.ts
--rw-r--r--   0 root         (0) root         (0)      640 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/pages.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.825245 peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/
--rw-r--r--   0 root         (0) root         (0)       57 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/index.ts
--rw-r--r--   0 root         (0) root         (0)    19057 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html
--rw-r--r--   0 root         (0) root         (0)      810 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss
--rw-r--r--   0 root         (0) root         (0)      513 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts
--rw-r--r--   0 root         (0) root         (0)      222 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/app/plugin-root.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/assets/
--rw-r--r--   0 root         (0) root         (0)   156480 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-Medium.ttf
--rw-r--r--   0 root         (0) root         (0)   158192 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   155192 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-SemiBold.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)    12054 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_docdb/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)    12730 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_search/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)     5572 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_user/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/environments/
--rw-r--r--   0 root         (0) root         (0)       54 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/environments/environment.prod.ts
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/environments/environment.ts
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app/src/environments/peek-app-environment.ts
--rw-r--r--   0 root         (0) root         (0)    39980 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     5317 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/index.html
--rw-r--r--   0 root         (0) root         (0)      883 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/main.ts
--rw-r--r--   0 root         (0) root         (0)     2395 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/polyfills.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.826245 peek-field-app-3.3.3/peek_field_app/src/styles/
--rw-r--r--   0 root         (0) root         (0)      227 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/styles/ant-design.scss
--rw-r--r--   0 root         (0) root         (0)     7181 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/styles/shared.scss
--rw-r--r--   0 root         (0) root         (0)     2251 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/styles/styles-layout.scss
--rw-r--r--   0 root         (0) root         (0)    33037 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/styles/theme.less
--rw-r--r--   0 root         (0) root         (0)     1593 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/styles.scss
--rw-r--r--   0 root         (0) root         (0)     1090 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/test.ts
--rw-r--r--   0 root         (0) root         (0)      521 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/tsconfig.app.json
--rw-r--r--   0 root         (0) root         (0)      242 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/tsconfig.spec.json
--rw-r--r--   0 root         (0) root         (0)      185 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/src/typings.d.ts
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)      320 2022-11-14 05:34:28.000000 peek-field-app-3.3.3/peek_field_app/tsconfig.worker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:02.816245 peek-field-app-3.3.3/peek_field_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)      360 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9949 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/peek_field_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:36:02.827246 peek-field-app-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3087 2022-11-14 05:36:02.000000 peek-field-app-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.826211 peek-field-app-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-12 11:04:45.826211 peek-field-app-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.816211 peek-field-app-3.4.0/peek_field_app/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/.browserslistrc
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/README.md
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.816211 peek-field-app-3.4.0/peek_field_app/android/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/.npmignore
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/build.gradle
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/capacitor.build.gradle
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/proguard-rules.pro
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/assets/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/assets/capacitor.config.json
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/assets/capacitor.plugins.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/com/synerty/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/com/synerty/peek/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable/
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     7705 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9251 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    17683 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     7934 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9875 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    13346 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.817211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-v24/
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/layout/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/layout/activity_main.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     3450 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     5036 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)     6593 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/
+-rw-r--r--   0 root         (0) root         (0)     6644 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)     9793 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)    10455 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/
+-rw-r--r--   0 root         (0) root         (0)     9441 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
+-rw-r--r--   0 root         (0) root         (0)    15529 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png
+-rw-r--r--   0 root         (0) root         (0)    15916 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.818211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/values/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/values/ic_launcher_background.xml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/values/strings.xml
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/values/styles.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/xml/
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/xml/config.xml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/xml/file_paths.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.813211 peek-field-app-3.4.0/peek_field_app/android/app/src/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.814211 peek-field-app-3.4.0/peek_field_app/android/app/src/test/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.814211 peek-field-app-3.4.0/peek_field_app/android/app/src/test/java/com/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.814211 peek-field-app-3.4.0/peek_field_app/android/app/src/test/java/com/getcapacitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/app/src/test/java/com/getcapacitor/myapp/ExampleUnitTest.java
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/build.gradle
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/capacitor.settings.gradle
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.814211 peek-field-app-3.4.0/peek_field_app/android/gradle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/android/gradle/wrapper/
+-rw-r--r--   0 root         (0) root         (0)    55616 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/gradle.properties
+-rwxr-xr-x   0 root         (0) root         (0)     5856 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/gradlew
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/gradlew.bat
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/settings.gradle
+-rw-r--r--   0 root         (0) root         (0)      562 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/android/variables.gradle
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/angular.json
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/capacitor.config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/e2e/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/e2e/app.e2e-spec.ts
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/e2e/app.po.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/e2e/tsconfig.e2e.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/ios/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/ios/App/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/ios/App/App/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/AppDelegate.swift
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.820211 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.821211 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@1x.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@2x.png
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-20x20@3x.png
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@1x.png
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@2x.png
+-rw-r--r--   0 root         (0) root         (0)    14448 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-29x29@3x.png
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@1x.png
+-rw-r--r--   0 root         (0) root         (0)    12478 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x-1.png
+-rw-r--r--   0 root         (0) root         (0)    12478 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26321 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-40x40@3x.png
+-rw-r--r--   0 root         (0) root         (0)  1769991 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-512@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26321 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@2x.png
+-rw-r--r--   0 root         (0) root         (0)    56548 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-60x60@3x.png
+-rw-r--r--   0 root         (0) root         (0)    11435 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@1x.png
+-rw-r--r--   0 root         (0) root         (0)    41291 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-76x76@2x.png
+-rw-r--r--   0 root         (0) root         (0)    48964 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/AppIcon-83.5x83.5@2x.png
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Contents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.822211 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/Contents.json
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png
+-rw-r--r--   0 root         (0) root         (0)    41273 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.822211 peek-field-app-3.4.0/peek_field_app/ios/App/App/Base.lproj/
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Base.lproj/Main.storyboard
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/Info.plist
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/capacitor.config.json
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App/config.xml
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App copy-Info.plist
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/
+-rw-r--r--   0 root         (0) root         (0)    17768 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/project.pbxproj
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.819211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.814211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/xcshareddata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.820211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.820211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcworkspace/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.820211 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcworkspace/xcshareddata/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/App.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/ios/App/Podfile
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/karma.conf.js
+-rw-r--r--   0 root         (0) root         (0)   675563 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app/package.json
+-rw-r--r--   0 root         (0) root         (0)      868 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/protractor.conf.js
+-rw-r--r--   0 root         (0) root         (0)      279 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/proxy.conf.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.822211 peek-field-app-3.4.0/peek_field_app/resources/
+-rw-r--r--   0 root         (0) root         (0)  1805857 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/resources/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.823211 peek-field-app-3.4.0/peek_field_app/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)    14824 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/scripts/build_capacitor_app.sh
+-rw-r--r--   0 root         (0) root         (0)      734 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/scripts/exportOptionsPlist.plist.template
+-rwxr-xr-x   0 root         (0) root         (0)     2601 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/scripts/prepare_capacitor_ios_app.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.823211 peek-field-app-3.4.0/peek_field_app/src/
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/_components.scss
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/_variables.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.823211 peek-field-app-3.4.0/peek_field_app/src/app/
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/app.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/app.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      834 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/app.services.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.823211 peek-field-app-3.4.0/peek_field_app/src/app/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/core/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/core/components/app/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/app/app.component.html
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/app/app.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/app/app.component.ts
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/components.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.html
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.ts
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/index.ts
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/index.ts
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/status.component.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/core/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.824211 peek-field-app-3.4.0/peek_field_app/src/app/pages/config/
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/config/config.page.html
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/config/config.page.scss
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/config/config.page.ts
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/config/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/app/pages/home/
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/home/home.page.html
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/home/home.page.scss
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/home/home.page.ts
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/home/index.ts
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/index.ts
+-rw-r--r--   0 root         (0) root         (0)      640 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/pages.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/index.ts
+-rw-r--r--   0 root         (0) root         (0)    19057 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html
+-rw-r--r--   0 root         (0) root         (0)      810 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/app/plugin-root.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/assets/
+-rw-r--r--   0 root         (0) root         (0)   156480 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-Medium.ttf
+-rw-r--r--   0 root         (0) root         (0)   158192 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   155192 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-SemiBold.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_docdb/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_search/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_user/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.825211 peek-field-app-3.4.0/peek_field_app/src/environments/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/environments/environment.prod.ts
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/environments/environment.ts
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app/src/environments/peek-app-environment.ts
+-rw-r--r--   0 root         (0) root         (0)    39980 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/index.html
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/main.ts
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/polyfills.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.826211 peek-field-app-3.4.0/peek_field_app/src/styles/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/styles/ant-design.scss
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/styles/shared.scss
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/styles/styles-layout.scss
+-rw-r--r--   0 root         (0) root         (0)    33037 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/styles/theme.less
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/styles.scss
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/test.ts
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/tsconfig.app.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/tsconfig.spec.json
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/src/typings.d.ts
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-12 11:03:19.000000 peek-field-app-3.4.0/peek_field_app/tsconfig.worker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:45.816211 peek-field-app-3.4.0/peek_field_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/peek_field_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:45.826211 peek-field-app-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-04-12 11:04:45.000000 peek-field-app-3.4.0/setup.py
```

### Comparing `peek-field-app-3.3.3/README.rst` & `peek-field-app-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/README.md` & `peek-field-app-3.4.0/peek_field_app/README.md`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/.gitignore` & `peek-field-app-3.4.0/peek_field_app/android/.gitignore`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/build.gradle` & `peek-field-app-3.4.0/peek_field_app/android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/capacitor.build.gradle` & `peek-field-app-3.4.0/peek_field_app/android/app/capacitor.build.gradle`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,24 @@
       targetCompatibility JavaVersion.VERSION_1_8
   }
 }
 
 apply from: "../capacitor-cordova-android-plugins/cordova.variables.gradle"
 dependencies {
     implementation project(':capacitor-community-background-geolocation')
+    implementation project(':capacitor-community-file-opener')
+    implementation project(':capacitor-community-http')
     implementation project(':capacitor-community-sqlite')
-    implementation project(':capacitor-device')
     implementation project(':capacitor-app')
-    implementation project(':capacitor-geolocation')
+    implementation project(':capacitor-browser')
+    implementation project(':capacitor-device')
     implementation project(':capacitor-dialog')
+    implementation project(':capacitor-filesystem')
+    implementation project(':capacitor-geolocation')
+    implementation project(':capacitor-local-notifications')
     implementation project(':capacitor-network')
 
 }
 
 
 if (hasProperty('postBuildExtras')) {
   postBuildExtras()
```

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/proguard-rules.pro` & `peek-field-app-3.4.0/peek_field_app/android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java` & `peek-field-app-3.4.0/peek_field_app/android/app/src/androidTest/java/com/getcapacitor/myapp/ExampleInstrumentedTest.java`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/AndroidManifest.xml` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/assets/capacitor.plugins.json` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/assets/capacitor.plugins.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {'10': "{'pkg': '@capacitor/local-notifications', 'classpath': "*

 * *       "'com.capacitorjs.plugins.localnotifications.LocalNotificationsPlugin'}",*

 * * '8': "{'pkg': '@capacitor/filesystem', 'classpath': "*

 * *      "'com.capacitorjs.plugins.filesystem.FilesystemPlugin'}",*

 * * 'insert': "[(1, OrderedDict([('pkg', '@capacitor-community/file-opener'), ('classpath', "*

 * *           "'com.ryltsov.alex.plugins.file.opener.FileOpenerPlugin')])), (2, OrderedDict([('pkg', "*

 * *           "'@capacitor-community/http'), ('classpath',  […]*

```diff
@@ -1,30 +1,50 @@
 [
     {
         "classpath": "com.equimaps.capacitor_background_geolocation.BackgroundGeolocation",
         "pkg": "@capacitor-community/background-geolocation"
     },
     {
+        "classpath": "com.ryltsov.alex.plugins.file.opener.FileOpenerPlugin",
+        "pkg": "@capacitor-community/file-opener"
+    },
+    {
+        "classpath": "com.getcapacitor.plugin.http.Http",
+        "pkg": "@capacitor-community/http"
+    },
+    {
         "classpath": "com.getcapacitor.community.database.sqlite.CapacitorSQLitePlugin",
         "pkg": "@capacitor-community/sqlite"
     },
     {
+        "classpath": "com.capacitorjs.plugins.app.AppPlugin",
+        "pkg": "@capacitor/app"
+    },
+    {
+        "classpath": "com.capacitorjs.plugins.browser.BrowserPlugin",
+        "pkg": "@capacitor/browser"
+    },
+    {
         "classpath": "com.capacitorjs.plugins.device.DevicePlugin",
         "pkg": "@capacitor/device"
     },
     {
-        "classpath": "com.capacitorjs.plugins.app.AppPlugin",
-        "pkg": "@capacitor/app"
+        "classpath": "com.capacitorjs.plugins.dialog.DialogPlugin",
+        "pkg": "@capacitor/dialog"
+    },
+    {
+        "classpath": "com.capacitorjs.plugins.filesystem.FilesystemPlugin",
+        "pkg": "@capacitor/filesystem"
     },
     {
         "classpath": "com.capacitorjs.plugins.geolocation.GeolocationPlugin",
         "pkg": "@capacitor/geolocation"
     },
     {
-        "classpath": "com.capacitorjs.plugins.dialog.DialogPlugin",
-        "pkg": "@capacitor/dialog"
+        "classpath": "com.capacitorjs.plugins.localnotifications.LocalNotificationsPlugin",
+        "pkg": "@capacitor/local-notifications"
     },
     {
         "classpath": "com.capacitorjs.plugins.network.NetworkPlugin",
         "pkg": "@capacitor/network"
     }
 ]
```

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/java/com/synerty/peek/MainActivity.java`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-hdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-mdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-land-xxxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-hdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-mdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-port-xxxhdpi/splash.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/drawable-v24/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/layout/activity_main.xml` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/layout/activity_main.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-hdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-mdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_foreground.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/app/src/main/res/values/styles.xml` & `peek-field-app-3.4.0/peek_field_app/android/app/src/main/res/values/styles.xml`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/build.gradle` & `peek-field-app-3.4.0/peek_field_app/android/build.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/capacitor.settings.gradle` & `peek-field-app-3.4.0/peek_field_app/android/capacitor.settings.gradle`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 // DO NOT EDIT THIS FILE! IT IS GENERATED EACH TIME "capacitor update" IS RUN
 include ':capacitor-android'
 project(':capacitor-android').projectDir = new File('../node_modules/@capacitor/android/capacitor')
 
 include ':capacitor-community-background-geolocation'
 project(':capacitor-community-background-geolocation').projectDir = new File('../node_modules/@capacitor-community/background-geolocation/android')
 
+include ':capacitor-community-file-opener'
+project(':capacitor-community-file-opener').projectDir = new File('../node_modules/@capacitor-community/file-opener/android')
+
+include ':capacitor-community-http'
+project(':capacitor-community-http').projectDir = new File('../node_modules/@capacitor-community/http/android')
+
 include ':capacitor-community-sqlite'
 project(':capacitor-community-sqlite').projectDir = new File('../node_modules/@capacitor-community/sqlite/android')
 
+include ':capacitor-app'
+project(':capacitor-app').projectDir = new File('../node_modules/@capacitor/app/android')
+
+include ':capacitor-browser'
+project(':capacitor-browser').projectDir = new File('../node_modules/@capacitor/browser/android')
+
 include ':capacitor-device'
 project(':capacitor-device').projectDir = new File('../node_modules/@capacitor/device/android')
 
-include ':capacitor-app'
-project(':capacitor-app').projectDir = new File('../node_modules/@capacitor/app/android')
+include ':capacitor-dialog'
+project(':capacitor-dialog').projectDir = new File('../node_modules/@capacitor/dialog/android')
+
+include ':capacitor-filesystem'
+project(':capacitor-filesystem').projectDir = new File('../node_modules/@capacitor/filesystem/android')
 
 include ':capacitor-geolocation'
 project(':capacitor-geolocation').projectDir = new File('../node_modules/@capacitor/geolocation/android')
 
-include ':capacitor-dialog'
-project(':capacitor-dialog').projectDir = new File('../node_modules/@capacitor/dialog/android')
+include ':capacitor-local-notifications'
+project(':capacitor-local-notifications').projectDir = new File('../node_modules/@capacitor/local-notifications/android')
 
 include ':capacitor-network'
 project(':capacitor-network').projectDir = new File('../node_modules/@capacitor/network/android')
```

### Comparing `peek-field-app-3.3.3/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar` & `peek-field-app-3.4.0/peek_field_app/android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/gradle.properties` & `peek-field-app-3.4.0/peek_field_app/android/gradle.properties`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/gradlew` & `peek-field-app-3.4.0/peek_field_app/android/gradlew`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/gradlew.bat` & `peek-field-app-3.4.0/peek_field_app/android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/android/variables.gradle` & `peek-field-app-3.4.0/peek_field_app/android/variables.gradle`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/angular.json` & `peek-field-app-3.4.0/peek_field_app/angular.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/AppDelegate.swift` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/AppDelegate.swift`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @UIApplicationMain
 class AppDelegate: UIResponder, UIApplicationDelegate {
 
   var window: UIWindow?
 
 
   func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
+    application.applicationSupportsShakeToEdit = false;
     // Override point for customization after application launch.
     return true
   }
 
   func applicationWillResignActive(_ application: UIApplication) {
     // Sent when the application is about to move from active to inactive state. This can occur for certain types of temporary interruptions (such as an incoming phone call or SMS message) or when the user quits the application and it begins the transition to the background state.
     // Use this method to pause ongoing tasks, disable timers, and invalidate graphics rendering callbacks. Games should use this method to pause the game.
```

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Base.lproj/Main.storyboard` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Info.plist` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Info.plist`

 * *Files 2% similar despite different names*

#### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App/Info.plist` & `peek-field-app-3.4.0/peek_field_app/ios/App/App/Info.plist`

```diff
@@ -3,69 +3,71 @@
   PUBLIC '-//Apple//DTD PLIST 1.0//EN'
   'http://www.apple.com/DTDs/PropertyList-1.0.dtd'>
 <plist version="1.0">
   <dict>
     <key>CFBundleDevelopmentRegion</key>
     <string>en</string>
     <key>CFBundleDisplayName</key>
-    <string>peek</string>
+    <string>$(DISPLAY_NAME)</string>
     <key>CFBundleExecutable</key>
     <string>$(EXECUTABLE_NAME)</string>
     <key>CFBundleIdentifier</key>
     <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
     <key>CFBundleInfoDictionaryVersion</key>
     <string>6.0</string>
     <key>CFBundleName</key>
-    <string>$(PRODUCT_NAME)</string>
+    <string>$(DISPLAY_NAME)</string>
     <key>CFBundlePackageType</key>
     <string>APPL</string>
     <key>CFBundleShortVersionString</key>
-    <string>3.2.2</string>
+    <string>$(MARKETING_VERSION)</string>
     <key>CFBundleURLTypes</key>
     <array>
       <dict>
         <key>CFBundleURLName</key>
         <string>com.getcapacitor.capacitor</string>
         <key>CFBundleURLSchemes</key>
         <array>
           <string>capacitor</string>
         </array>
       </dict>
     </array>
     <key>CFBundleVersion</key>
-    <string>b2205172235</string>
+    <string>$(CURRENT_PROJECT_VERSION)</string>
     <key>LSRequiresIPhoneOS</key>
     <true/>
+    <key>LSSupportsOpeningDocumentsInPlace</key>
+    <true/>
     <key>NSAppTransportSecurity</key>
     <dict>
       <key>NSAllowsArbitraryLoads</key>
       <true/>
     </dict>
     <key>NSCameraUsageDescription</key>
     <string>NSCameraUsageDescription</string>
     <key>NSLocationAlwaysAndWhenInUseUsageDescription</key>
     <string>Location required when app is in use</string>
     <key>NSLocationAlwaysUsageDescription</key>
     <string>Location required when app is in use</string>
-    <key>NSLocationWhenInUseUsageDescription</key>
-    <string>Location required in background</string>
     <key>NSMicrophoneUsageDescription</key>
     <string>To Record Audio With Video</string>
     <key>NSMotionUsageDescription</key>
     <string>Motion permission helps detect when device in in-motion</string>
     <key>NSPhotoLibraryAddUsageDescription</key>
     <string>NSPhotoLibraryAddUsageDescription</string>
     <key>NSPhotoLibraryUsageDescription</key>
     <string>NSPhotoLibraryUsageDescription</string>
     <key>UIBackgroundModes</key>
     <array>
       <string>fetch</string>
       <string>location</string>
       <string>processing</string>
     </array>
+    <key>UIFileSharingEnabled</key>
+    <true/>
     <key>UILaunchStoryboardName</key>
     <string>LaunchScreen</string>
     <key>UIMainStoryboardFile</key>
     <string>Main</string>
     <key>UIRequiredDeviceCapabilities</key>
     <array>
       <string>armv7</string>
```

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App copy-Info.plist` & `peek-field-app-3.4.0/peek_field_app/ios/App/App copy-Info.plist`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/project.pbxproj` & `peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/project.pbxproj`

 * *Files 15% similar despite different names*

```diff
@@ -3,56 +3,59 @@
 	archiveVersion = 1;
 	classes = {
 	};
 	objectVersion = 48;
 	objects = {
 
 /* Begin PBXBuildFile section */
+		1736EADA6A289AF35C4CCED2 /* Pods_peek.framework in Frameworks */ = {isa = PBXBuildFile; fileRef = 9C3EFF21D8277CF1CDFB6819 /* Pods_peek.framework */; };
 		2FAD9763203C412B000D30F8 /* config.xml in Resources */ = {isa = PBXBuildFile; fileRef = 2FAD9762203C412B000D30F8 /* config.xml */; };
 		50379B232058CBB4000EE86E /* capacitor.config.json in Resources */ = {isa = PBXBuildFile; fileRef = 50379B222058CBB4000EE86E /* capacitor.config.json */; };
 		504EC3081FED79650016851F /* AppDelegate.swift in Sources */ = {isa = PBXBuildFile; fileRef = 504EC3071FED79650016851F /* AppDelegate.swift */; };
 		504EC30D1FED79650016851F /* Main.storyboard in Resources */ = {isa = PBXBuildFile; fileRef = 504EC30B1FED79650016851F /* Main.storyboard */; };
 		504EC30F1FED79650016851F /* Assets.xcassets in Resources */ = {isa = PBXBuildFile; fileRef = 504EC30E1FED79650016851F /* Assets.xcassets */; };
 		504EC3121FED79650016851F /* LaunchScreen.storyboard in Resources */ = {isa = PBXBuildFile; fileRef = 504EC3101FED79650016851F /* LaunchScreen.storyboard */; };
 		50B271D11FEDC1A000F3C39B /* public in Resources */ = {isa = PBXBuildFile; fileRef = 50B271D01FEDC1A000F3C39B /* public */; };
-		A084ECDBA7D38E1E42DFC39D /* Pods_App.framework in Frameworks */ = {isa = PBXBuildFile; fileRef = AF277DCFFFF123FFC6DF26C7 /* Pods_App.framework */; };
 /* End PBXBuildFile section */
 
 /* Begin PBXFileReference section */
+		03FE1A041BEAAED37F1D24F4 /* Pods-peek.release.xcconfig */ = {isa = PBXFileReference; includeInIndex = 1; lastKnownFileType = text.xcconfig; name = "Pods-peek.release.xcconfig"; path = "Pods/Target Support Files/Pods-peek/Pods-peek.release.xcconfig"; sourceTree = "<group>"; };
 		2FAD9762203C412B000D30F8 /* config.xml */ = {isa = PBXFileReference; lastKnownFileType = text.xml; path = config.xml; sourceTree = "<group>"; };
 		50379B222058CBB4000EE86E /* capacitor.config.json */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = text.json; path = capacitor.config.json; sourceTree = "<group>"; };
-		504EC3041FED79650016851F /* App.app */ = {isa = PBXFileReference; explicitFileType = wrapper.application; includeInIndex = 0; path = App.app; sourceTree = BUILT_PRODUCTS_DIR; };
+		504EC3041FED79650016851F /* peek.app */ = {isa = PBXFileReference; explicitFileType = wrapper.application; includeInIndex = 0; path = peek.app; sourceTree = BUILT_PRODUCTS_DIR; };
 		504EC3071FED79650016851F /* AppDelegate.swift */ = {isa = PBXFileReference; lastKnownFileType = sourcecode.swift; path = AppDelegate.swift; sourceTree = "<group>"; };
 		504EC30C1FED79650016851F /* Base */ = {isa = PBXFileReference; lastKnownFileType = file.storyboard; name = Base; path = Base.lproj/Main.storyboard; sourceTree = "<group>"; };
 		504EC30E1FED79650016851F /* Assets.xcassets */ = {isa = PBXFileReference; lastKnownFileType = folder.assetcatalog; path = Assets.xcassets; sourceTree = "<group>"; };
 		504EC3111FED79650016851F /* Base */ = {isa = PBXFileReference; lastKnownFileType = file.storyboard; name = Base; path = Base.lproj/LaunchScreen.storyboard; sourceTree = "<group>"; };
 		504EC3131FED79650016851F /* Info.plist */ = {isa = PBXFileReference; lastKnownFileType = text.plist.xml; path = Info.plist; sourceTree = "<group>"; };
 		50B271D01FEDC1A000F3C39B /* public */ = {isa = PBXFileReference; lastKnownFileType = folder; path = public; sourceTree = SOURCE_ROOT; };
+		6863DA97C9F3B5AEF3B7F3C9 /* Pods-peek.debug.xcconfig */ = {isa = PBXFileReference; includeInIndex = 1; lastKnownFileType = text.xcconfig; name = "Pods-peek.debug.xcconfig"; path = "Pods/Target Support Files/Pods-peek/Pods-peek.debug.xcconfig"; sourceTree = "<group>"; };
 		780558BD251DC73F00E949E3 /* App copy-Info.plist */ = {isa = PBXFileReference; lastKnownFileType = text.plist.xml; name = "App copy-Info.plist"; path = "/Users/jsorrell/dev-peek/peek-field-app/peek_field_app/ios/App/App copy-Info.plist"; sourceTree = "<absolute>"; };
-		AF277DCFFFF123FFC6DF26C7 /* Pods_App.framework */ = {isa = PBXFileReference; explicitFileType = wrapper.framework; includeInIndex = 0; path = Pods_App.framework; sourceTree = BUILT_PRODUCTS_DIR; };
+		9C3EFF21D8277CF1CDFB6819 /* Pods_peek.framework */ = {isa = PBXFileReference; explicitFileType = wrapper.framework; includeInIndex = 0; path = Pods_peek.framework; sourceTree = BUILT_PRODUCTS_DIR; };
 		AF51FD2D460BCFE21FA515B2 /* Pods-App.release.xcconfig */ = {isa = PBXFileReference; includeInIndex = 1; lastKnownFileType = text.xcconfig; name = "Pods-App.release.xcconfig"; path = "Pods/Target Support Files/Pods-App/Pods-App.release.xcconfig"; sourceTree = "<group>"; };
+		BF3004557781B76C72682F2D /* Pods-peek.debug.xcconfig */ = {isa = PBXFileReference; includeInIndex = 1; lastKnownFileType = text.xcconfig; name = "Pods-peek.debug.xcconfig"; path = "Pods/Target Support Files/Pods-peek/Pods-peek.debug.xcconfig"; sourceTree = "<group>"; };
 		FC68EB0AF532CFC21C3344DD /* Pods-App.debug.xcconfig */ = {isa = PBXFileReference; includeInIndex = 1; lastKnownFileType = text.xcconfig; name = "Pods-App.debug.xcconfig"; path = "Pods/Target Support Files/Pods-App/Pods-App.debug.xcconfig"; sourceTree = "<group>"; };
 /* End PBXFileReference section */
 
 /* Begin PBXFrameworksBuildPhase section */
 		504EC3011FED79650016851F /* Frameworks */ = {
 			isa = PBXFrameworksBuildPhase;
 			buildActionMask = 2147483647;
 			files = (
-				A084ECDBA7D38E1E42DFC39D /* Pods_App.framework in Frameworks */,
+				1736EADA6A289AF35C4CCED2 /* Pods_peek.framework in Frameworks */,
 			);
 			runOnlyForDeploymentPostprocessing = 0;
 		};
 /* End PBXFrameworksBuildPhase section */
 
 /* Begin PBXGroup section */
 		27E2DDA53C4D2A4D1A88CE4A /* Frameworks */ = {
 			isa = PBXGroup;
 			children = (
-				AF277DCFFFF123FFC6DF26C7 /* Pods_App.framework */,
+				9C3EFF21D8277CF1CDFB6819 /* Pods_peek.framework */,
 			);
 			name = Frameworks;
 			sourceTree = "<group>";
 		};
 		504EC2FB1FED79650016851F = {
 			isa = PBXGroup;
 			children = (
@@ -63,15 +66,15 @@
 				780558BD251DC73F00E949E3 /* App copy-Info.plist */,
 			);
 			sourceTree = "<group>";
 		};
 		504EC3051FED79650016851F /* Products */ = {
 			isa = PBXGroup;
 			children = (
-				504EC3041FED79650016851F /* App.app */,
+				504EC3041FED79650016851F /* peek.app */,
 			);
 			name = Products;
 			sourceTree = "<group>";
 		};
 		504EC3061FED79650016851F /* App */ = {
 			isa = PBXGroup;
 			children = (
@@ -88,38 +91,40 @@
 			sourceTree = "<group>";
 		};
 		7F8756D8B27F46E3366F6CEA /* Pods */ = {
 			isa = PBXGroup;
 			children = (
 				FC68EB0AF532CFC21C3344DD /* Pods-App.debug.xcconfig */,
 				AF51FD2D460BCFE21FA515B2 /* Pods-App.release.xcconfig */,
+				6863DA97C9F3B5AEF3B7F3C9 /* Pods-peek.debug.xcconfig */,
+				03FE1A041BEAAED37F1D24F4 /* Pods-peek.release.xcconfig */,
 			);
 			name = Pods;
 			sourceTree = "<group>";
 		};
 /* End PBXGroup section */
 
 /* Begin PBXNativeTarget section */
-		504EC3031FED79650016851F /* App */ = {
+		504EC3031FED79650016851F /* peek */ = {
 			isa = PBXNativeTarget;
-			buildConfigurationList = 504EC3161FED79650016851F /* Build configuration list for PBXNativeTarget "App" */;
+			buildConfigurationList = 504EC3161FED79650016851F /* Build configuration list for PBXNativeTarget "peek" */;
 			buildPhases = (
 				6634F4EFEBD30273BCE97C65 /* [CP] Check Pods Manifest.lock */,
 				504EC3001FED79650016851F /* Sources */,
 				504EC3011FED79650016851F /* Frameworks */,
 				504EC3021FED79650016851F /* Resources */,
 				9592DBEFFC6D2A0C8D5DEB22 /* [CP] Embed Pods Frameworks */,
 			);
 			buildRules = (
 			);
 			dependencies = (
 			);
-			name = App;
+			name = peek;
 			productName = App;
-			productReference = 504EC3041FED79650016851F /* App.app */;
+			productReference = 504EC3041FED79650016851F /* peek.app */;
 			productType = "com.apple.product-type.application";
 		};
 /* End PBXNativeTarget section */
 
 /* Begin PBXProject section */
 		504EC2FC1FED79650016851F /* Project object */ = {
 			isa = PBXProject;
@@ -143,15 +148,15 @@
 				Base,
 			);
 			mainGroup = 504EC2FB1FED79650016851F;
 			productRefGroup = 504EC3051FED79650016851F /* Products */;
 			projectDirPath = "";
 			projectRoot = "";
 			targets = (
-				504EC3031FED79650016851F /* App */,
+				504EC3031FED79650016851F /* peek */,
 			);
 		};
 /* End PBXProject section */
 
 /* Begin PBXResourcesBuildPhase section */
 		504EC3021FED79650016851F /* Resources */ = {
 			isa = PBXResourcesBuildPhase;
@@ -176,15 +181,15 @@
 			);
 			inputPaths = (
 				"${PODS_PODFILE_DIR_PATH}/Podfile.lock",
 				"${PODS_ROOT}/Manifest.lock",
 			);
 			name = "[CP] Check Pods Manifest.lock";
 			outputPaths = (
-				"$(DERIVED_FILE_DIR)/Pods-App-checkManifestLockResult.txt",
+				"$(DERIVED_FILE_DIR)/Pods-peek-checkManifestLockResult.txt",
 			);
 			runOnlyForDeploymentPostprocessing = 0;
 			shellPath = /bin/sh;
 			shellScript = "diff \"${PODS_PODFILE_DIR_PATH}/Podfile.lock\" \"${PODS_ROOT}/Manifest.lock\" > /dev/null\nif [ $? != 0 ] ; then\n    # print error to STDERR\n    echo \"error: The sandbox is not in sync with the Podfile.lock. Run 'pod install' or update your CocoaPods installation.\" >&2\n    exit 1\nfi\n# This output is used by Xcode 'outputs' to avoid re-running this script phase.\necho \"SUCCESS\" > \"${SCRIPT_OUTPUT_FILE_0}\"\n";
 			showEnvVarsInLog = 0;
 		};
 		9592DBEFFC6D2A0C8D5DEB22 /* [CP] Embed Pods Frameworks */ = {
@@ -195,15 +200,15 @@
 			inputPaths = (
 			);
 			name = "[CP] Embed Pods Frameworks";
 			outputPaths = (
 			);
 			runOnlyForDeploymentPostprocessing = 0;
 			shellPath = /bin/sh;
-			shellScript = "\"${PODS_ROOT}/Target Support Files/Pods-App/Pods-App-frameworks.sh\"\n";
+			shellScript = "\"${PODS_ROOT}/Target Support Files/Pods-peek/Pods-peek-frameworks.sh\"\n";
 			showEnvVarsInLog = 0;
 		};
 /* End PBXShellScriptBuildPhase section */
 
 /* Begin PBXSourcesBuildPhase section */
 		504EC3001FED79650016851F /* Sources */ = {
 			isa = PBXSourcesBuildPhase;
@@ -342,15 +347,15 @@
 				TARGETED_DEVICE_FAMILY = 2;
 				VALIDATE_PRODUCT = YES;
 			};
 			name = Release;
 		};
 		504EC3171FED79650016851F /* Debug */ = {
 			isa = XCBuildConfiguration;
-			baseConfigurationReference = FC68EB0AF532CFC21C3344DD /* Pods-App.debug.xcconfig */;
+			baseConfigurationReference = 6863DA97C9F3B5AEF3B7F3C9 /* Pods-peek.debug.xcconfig */;
 			buildSettings = {
 				ASSETCATALOG_COMPILER_APPICON_NAME = AppIcon;
 				CODE_SIGN_STYLE = Automatic;
 				CURRENT_PROJECT_VERSION = 2205240400;
 				DEVELOPMENT_TEAM = Q55F59LQD3;
 				INFOPLIST_FILE = App/Info.plist;
 				IPHONEOS_DEPLOYMENT_TARGET = 12.0;
@@ -363,15 +368,15 @@
 				SWIFT_VERSION = 5.0;
 				TARGETED_DEVICE_FAMILY = 2;
 			};
 			name = Debug;
 		};
 		504EC3181FED79650016851F /* Release */ = {
 			isa = XCBuildConfiguration;
-			baseConfigurationReference = AF51FD2D460BCFE21FA515B2 /* Pods-App.release.xcconfig */;
+			baseConfigurationReference = 03FE1A041BEAAED37F1D24F4 /* Pods-peek.release.xcconfig */;
 			buildSettings = {
 				ASSETCATALOG_COMPILER_APPICON_NAME = AppIcon;
 				CODE_SIGN_STYLE = Automatic;
 				CURRENT_PROJECT_VERSION = 2205240400;
 				DEVELOPMENT_TEAM = Q55F59LQD3;
 				INFOPLIST_FILE = App/Info.plist;
 				IPHONEOS_DEPLOYMENT_TARGET = 12.0;
@@ -393,15 +398,15 @@
 			buildConfigurations = (
 				504EC3141FED79650016851F /* Debug */,
 				504EC3151FED79650016851F /* Release */,
 			);
 			defaultConfigurationIsVisible = 0;
 			defaultConfigurationName = Release;
 		};
-		504EC3161FED79650016851F /* Build configuration list for PBXNativeTarget "App" */ = {
+		504EC3161FED79650016851F /* Build configuration list for PBXNativeTarget "peek" */ = {
 			isa = XCConfigurationList;
 			buildConfigurations = (
 				504EC3171FED79650016851F /* Debug */,
 				504EC3181FED79650016851F /* Release */,
 			);
 			defaultConfigurationIsVisible = 0;
 			defaultConfigurationName = Release;
```

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme` & `peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme`

 * *Files 3% similar despite different names*

#### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme` & `peek-field-app-3.4.0/peek_field_app/ios/App/App.xcodeproj/xcshareddata/xcschemes/App.xcscheme`

```diff
@@ -1,25 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <Scheme LastUpgradeVersion="1160" version="1.3">
   <BuildAction parallelizeBuildables="YES" buildImplicitDependencies="YES">
     <BuildActionEntries>
       <BuildActionEntry buildForTesting="YES" buildForRunning="YES" buildForProfiling="YES" buildForArchiving="YES" buildForAnalyzing="YES">
-        <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="App.app" BlueprintName="App" ReferencedContainer="container:App.xcodeproj"/>
+        <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="peek.app" BlueprintName="peek" ReferencedContainer="container:App.xcodeproj"/>
       </BuildActionEntry>
     </BuildActionEntries>
   </BuildAction>
   <TestAction buildConfiguration="Debug" selectedDebuggerIdentifier="Xcode.DebuggerFoundation.Debugger.LLDB" selectedLauncherIdentifier="Xcode.DebuggerFoundation.Launcher.LLDB" shouldUseLaunchSchemeArgsEnv="YES">
     <Testables/>
   </TestAction>
   <LaunchAction buildConfiguration="Debug" selectedDebuggerIdentifier="Xcode.DebuggerFoundation.Debugger.LLDB" selectedLauncherIdentifier="Xcode.DebuggerFoundation.Launcher.LLDB" launchStyle="0" useCustomWorkingDirectory="NO" ignoresPersistentStateOnLaunch="NO" debugDocumentVersioning="YES" debugServiceExtension="internal" allowLocationSimulation="YES">
     <BuildableProductRunnable runnableDebuggingMode="0">
-      <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="App.app" BlueprintName="App" ReferencedContainer="container:App.xcodeproj"/>
+      <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="peek.app" BlueprintName="peek" ReferencedContainer="container:App.xcodeproj"/>
     </BuildableProductRunnable>
   </LaunchAction>
   <ProfileAction buildConfiguration="Release" shouldUseLaunchSchemeArgsEnv="YES" savedToolIdentifier="" useCustomWorkingDirectory="NO" debugDocumentVersioning="YES">
     <BuildableProductRunnable runnableDebuggingMode="0">
-      <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="App.app" BlueprintName="App" ReferencedContainer="container:App.xcodeproj"/>
+      <BuildableReference BuildableIdentifier="primary" BlueprintIdentifier="504EC3031FED79650016851F" BuildableName="peek.app" BlueprintName="peek" ReferencedContainer="container:App.xcodeproj"/>
     </BuildableProductRunnable>
   </ProfileAction>
   <AnalyzeAction buildConfiguration="Debug"/>
   <ArchiveAction buildConfiguration="Release" revealArchiveInOrganizer="YES"/>
 </Scheme>
```

### Comparing `peek-field-app-3.3.3/peek_field_app/ios/App/Podfile` & `peek-field-app-3.4.0/peek_field_app/ios/App/Podfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-platform :ios, '12.0'
+platform :ios, '13.0'
 use_frameworks!
 
 # workaround to avoid Xcode caching of Pods that requires
 # Product -> Clean Build Folder after new Cordova plugins installed
 # Requires CocoaPods 1.6 or newer
 install! 'cocoapods', :disable_input_output_paths => true
 
 def capacitor_pods
   pod 'Capacitor', :path => '../../node_modules/@capacitor/ios'
   pod 'CapacitorCordova', :path => '../../node_modules/@capacitor/ios'
   pod 'CapacitorCommunityBackgroundGeolocation', :path => '../../node_modules/@capacitor-community/background-geolocation'
+  pod 'CapacitorCommunityFileOpener', :path => '../../node_modules/@capacitor-community/file-opener'
+  pod 'CapacitorCommunityHttp', :path => '../../node_modules/@capacitor-community/http'
   pod 'CapacitorCommunitySqlite', :path => '../../node_modules/@capacitor-community/sqlite'
-  pod 'CapacitorDevice', :path => '../../node_modules/@capacitor/device'
   pod 'CapacitorApp', :path => '../../node_modules/@capacitor/app'
-  pod 'CapacitorGeolocation', :path => '../../node_modules/@capacitor/geolocation'
+  pod 'CapacitorBrowser', :path => '../../node_modules/@capacitor/browser'
+  pod 'CapacitorDevice', :path => '../../node_modules/@capacitor/device'
   pod 'CapacitorDialog', :path => '../../node_modules/@capacitor/dialog'
+  pod 'CapacitorFilesystem', :path => '../../node_modules/@capacitor/filesystem'
+  pod 'CapacitorGeolocation', :path => '../../node_modules/@capacitor/geolocation'
+  pod 'CapacitorLocalNotifications', :path => '../../node_modules/@capacitor/local-notifications'
   pod 'CapacitorNetwork', :path => '../../node_modules/@capacitor/network'
   pod 'CordovaPlugins', :path => '../capacitor-cordova-ios-plugins'
 end
 
-target 'App' do
+target 'peek' do
   capacitor_pods
   # Add your Pods here
 end
```

### Comparing `peek-field-app-3.3.3/peek_field_app/karma.conf.js` & `peek-field-app-3.4.0/peek_field_app/karma.conf.js`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/package-lock.json` & `peek-field-app-3.4.0/peek_field_app/package-lock.json`

 * *Files identical despite different names*

#### Pretty-printed

 * *Similarity: 0.9996202098540146%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': {'version': '3.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-SE4PvtrpdAVfwarFAYJkAzpiwjFyxDhdnQxS8C2y2vN1mLV5yE1J7mPExOyQIMwXFbCdO+GtUHuBgpIk+WVUDg==', "*

 * *                   "'dependencies': {'tslib': {'version': '2.5.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz', 'integrity': "*

 * *                   […]*

```diff
@@ -1728,14 +1728,30 @@
             "version": "7.12.1"
         },
         "@capacitor-community/background-geolocation": {
             "integrity": "sha512-2dbTAjcSibf1OYl66KqH3Yhh9cBqhvppJlcV5Z6BMgPqccPcPTipPCoQpWdTIc8fZfKjSUD5DVDZjPMbRV3cTw==",
             "resolved": "https://registry.npmjs.org/@capacitor-community/background-geolocation/-/background-geolocation-1.2.1.tgz",
             "version": "1.2.1"
         },
+        "@capacitor-community/file-opener": {
+            "integrity": "sha512-tNxt6HeyPYW5Q0ZarEIG2uBbWEtLYpUnEyyxWXobWccXqJegT19KXwX53/vbzPBy56Z8pEQR8RavRnJOSha1Eg==",
+            "resolved": "https://registry.npmjs.org/@capacitor-community/file-opener/-/file-opener-1.0.4.tgz",
+            "version": "1.0.4"
+        },
+        "@capacitor-community/http": {
+            "integrity": "sha512-+pCkBXrwfm97UfjOgjV950H/qZ8SE36Mrcb46BlL1ps3VIsGuIO+AulL8GqTC6LewheRVtGJpRspNtneXQotNA==",
+            "requires": {
+                "@capacitor/android": "^3.0.0",
+                "@capacitor/core": "^3.0.0",
+                "@capacitor/filesystem": "^1.0.0",
+                "@capacitor/ios": "^3.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/@capacitor-community/http/-/http-1.4.1.tgz",
+            "version": "1.4.1"
+        },
         "@capacitor-community/sqlite": {
             "integrity": "sha512-51ZW+CQoXnuW8HXgVsUfXS+rvUQaVp3LthLKEj0o+1n2sC5A3hJm6w6+nL/1tgvyJi00Pj8uB9IKKqE6E+qIeg==",
             "requires": {
                 "jeep-sqlite": "^1.5.2"
             },
             "resolved": "https://registry.npmjs.org/@capacitor-community/sqlite/-/sqlite-3.5.1-1.tgz",
             "version": "3.5.1-1"
@@ -1746,14 +1762,19 @@
             "version": "3.5.1"
         },
         "@capacitor/app": {
             "integrity": "sha512-8ADkldHnoE1xkWvPUsGlERVGm6/Zvcxy6hCI80AxydIKyaCG7kbDAvUclebbnw/eFRxj2zBoVatGLjmJNvTbYw==",
             "resolved": "https://registry.npmjs.org/@capacitor/app/-/app-1.1.1.tgz",
             "version": "1.1.1"
         },
+        "@capacitor/browser": {
+            "integrity": "sha512-ni8IjsPyFUYqQ2JxBwzI7VpJUZHPr7QiRds5hQWM/1cpfH0+DWvjWHwzxQXuSbW0h+QGXGSJ/vwqjRns7NzLfQ==",
+            "resolved": "https://registry.npmjs.org/@capacitor/browser/-/browser-1.0.7.tgz",
+            "version": "1.0.7"
+        },
         "@capacitor/cli": {
             "dependencies": {
                 "commander": {
                     "integrity": "sha512-U7VdrJFnJgo4xjrHpTzu0yrHPGImdsmD95ZlgYSEajAn2JKzDhDTPG9kBTefmObL2w/ngeZnilk+OV9CG3d7UA==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-6.2.1.tgz",
                     "version": "6.2.1"
                 },
@@ -1841,14 +1862,19 @@
             "version": "1.1.2"
         },
         "@capacitor/dialog": {
             "integrity": "sha512-+B6lKlqlpZk9uDrHEYk2rj+b3DF1kxCqV+vGtKwNMr2tFvNppZVkYdZU+L503yAoFFejqgQ27n0A4vXg+BTcBQ==",
             "resolved": "https://registry.npmjs.org/@capacitor/dialog/-/dialog-1.0.7.tgz",
             "version": "1.0.7"
         },
+        "@capacitor/filesystem": {
+            "integrity": "sha512-8O3UuvL8HNUEJvZnmn8yUmvgB1evtXfcF0oxIo3YbSlylqywJwS3JTiuhKmsvSxCdpbTy8IaTsutVh3gZgWbKg==",
+            "resolved": "https://registry.npmjs.org/@capacitor/filesystem/-/filesystem-1.1.0.tgz",
+            "version": "1.1.0"
+        },
         "@capacitor/geolocation": {
             "integrity": "sha512-3u9Hu4E0VBMa6r0d2t9MENDIR+bv5Tf144uPmb2Bl7XLQeFwvu4BSp2neNq39x58PvcROPMNX1BOTSGpQep+1Q==",
             "resolved": "https://registry.npmjs.org/@capacitor/geolocation/-/geolocation-1.3.1.tgz",
             "version": "1.3.1"
         },
         "@capacitor/ios": {
             "integrity": "sha512-295L9dHe/QaejUpGI8Pxwb1i2yVgick1ExIDK26xk+tk1km3B1HVjsIS8qkf2SOp7tuwP9+W5T5p7rLMNN4v5g==",
@@ -2260,25 +2286,25 @@
             },
             "resolved": "https://registry.npmjs.org/@synerty/peek-plugin-base-js/-/peek-plugin-base-js-10.7.10.tgz",
             "version": "10.7.10"
         },
         "@synerty/vortexjs": {
             "dependencies": {
                 "tslib": {
-                    "integrity": "sha512-d6xOpEDfsi2CZVlPQzGeux8XMwLT9hssAsaPYExaQMuYskwb+x1x7J371tWlbBdWHroy99KnVB6qIkUbs5X3UQ==",
-                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.4.0.tgz",
-                    "version": "2.4.0"
+                    "integrity": "sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==",
+                    "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz",
+                    "version": "2.5.0"
                 }
             },
-            "integrity": "sha512-mH7pbrJfx8C16cHCdPFbzMpSGq9An2BKZjUwzzMfnemHksujYO+xXtOTbKHrY/tu/xXaSYUEzgbzr8aTqqOs1Q==",
+            "integrity": "sha512-SE4PvtrpdAVfwarFAYJkAzpiwjFyxDhdnQxS8C2y2vN1mLV5yE1J7mPExOyQIMwXFbCdO+GtUHuBgpIk+WVUDg==",
             "requires": {
                 "tslib": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.2.5.tgz",
-            "version": "3.2.5"
+            "resolved": "https://registry.npmjs.org/@synerty/vortexjs/-/vortexjs-3.3.3.tgz",
+            "version": "3.3.3"
         },
         "@types/cordova": {
             "integrity": "sha512-rkiiTuf/z2wTd4RxFOb+clE7PF4AEJU0hsczbUdkHHBtkUmpWQpEddynNfJYKYtZFJKbq4F+brfekt1kx85IZA==",
             "resolved": "https://registry.npmjs.org/@types/cordova/-/cordova-0.0.34.tgz",
             "version": "0.0.34"
         },
         "@types/emscripten": {
```

### Comparing `peek-field-app-3.3.3/peek_field_app/package.json` & `peek-field-app-3.4.0/peek_field_app/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9155328798185941%*

 * *Differences: {"'dependencies'": "{'@synerty/vortexjs': '^3.3.3', 'angular-svg-icon': '^13.4.0', "*

 * *                   "'@capacitor-community/file-opener': '^1.0.4', '@capacitor-community/http': "*

 * *                   "'^1.4.1', '@capacitor/browser': '^1.0.7', '@capacitor/filesystem': '^1.1.0'}",*

 * * "'scripts'": "{'start': 'ng serve --disableHostCheck --host 3.4.0.0 --port 4000 --proxy-config "*

 * *              "proxy.conf.json'}",*

 * * "'version'": "'3.4.0'"}*

```diff
@@ -8,29 +8,33 @@
         "@angular/forms": "^10.2.0",
         "@angular/platform-browser": "^10.2.0",
         "@angular/platform-browser-dynamic": "^10.2.0",
         "@angular/router": "^10.2.0",
         "@awesome-cordova-plugins/core": "^5.41.0",
         "@awesome-cordova-plugins/native-audio": "^5.41.0",
         "@capacitor-community/background-geolocation": "^1.2.1",
+        "@capacitor-community/file-opener": "^1.0.4",
+        "@capacitor-community/http": "^1.4.1",
         "@capacitor-community/sqlite": "^3.5.1-1",
         "@capacitor/android": "^3.5.1",
         "@capacitor/app": "^1.1.1",
+        "@capacitor/browser": "^1.0.7",
         "@capacitor/cli": "^3.5.1",
         "@capacitor/core": "^3.5.1",
         "@capacitor/device": "^1.1.2",
         "@capacitor/dialog": "^1.0.7",
+        "@capacitor/filesystem": "^1.1.0",
         "@capacitor/geolocation": "^1.3.1",
         "@capacitor/ios": "^3.5.1",
         "@capacitor/local-notifications": "^1.1.0",
         "@capacitor/network": "^1.0.7",
         "@ionic/pwa-elements": "^3.1.1",
         "@synerty/peek-plugin-base-js": "^10.7.10",
-        "@synerty/vortexjs": "^3.2.5",
-        "angular-svg-icon": "^13.3.3",
+        "@synerty/vortexjs": "^3.3.3",
+        "angular-svg-icon": "^13.4.0",
         "base-64": "^1.0.0",
         "bootstrap": "^3.3.7",
         "cordova-open-native-settings": "^1.5.5",
         "cordova-plugin-nativeaudio": "^3.0.9",
         "core-js": "^3.6.5",
         "jquery": "^3.3.1",
         "json-stable-stringify": "^1.0.1",
@@ -69,12 +73,12 @@
     "private": true,
     "scripts": {
         "build": "ng build",
         "e2e": "ng e2e",
         "lint": "ng lint",
         "ng": "ng",
         "postinstall": "ngcc --properties es2015 es5 browser module main --first-only --create-ivy-entry-points",
-        "start": "ng serve --disableHostCheck --host 3.3.3.0 --port 4000 --proxy-config proxy.conf.json",
+        "start": "ng serve --disableHostCheck --host 3.4.0.0 --port 4000 --proxy-config proxy.conf.json",
         "test": "ng test"
     },
-    "version": "3.3.3"
+    "version": "3.4.0"
 }
```

### Comparing `peek-field-app-3.3.3/peek_field_app/protractor.conf.js` & `peek-field-app-3.4.0/peek_field_app/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/scripts/build_capacitor_app.sh` & `peek-field-app-3.4.0/peek_field_app/scripts/build_capacitor_app.sh`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/scripts/exportOptionsPlist.plist.template` & `peek-field-app-3.4.0/peek_field_app/scripts/exportOptionsPlist.plist.template`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/scripts/prepare_capacitor_ios_app.sh` & `peek-field-app-3.4.0/peek_field_app/scripts/prepare_capacitor_ios_app.sh`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/_components.scss` & `peek-field-app-3.4.0/peek_field_app/src/_components.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/_variables.scss` & `peek-field-app-3.4.0/peek_field_app/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/app.module.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/app.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/app.routes.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/app.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/app.services.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/app.services.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/app/app.component.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/app/app.component.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/components.module.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/components.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.html` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.html`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,17 @@
                     nzStyle="backgroundColor: #faad14"
                 >
                     <i
                         nz-icon
                         nzTheme="outline"
                         nzType="home"
                         style="line-height: inherit; padding: 2px"
+                        [class.slow-network]="
+                            deviceStatusService.isNetworkSlow$ | async
+                        "
                     ></i>
                 </nz-badge>
             </button>
             <button
                 *ngFor="let link of headerService.links$ | async"
                 [routerLink]="[link.resourcePath]"
             >
```

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.scss` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 @import "src/variables";
 
+.slow-network {
+    color: orange;
+}
 :host {
     .peek-header-component {
         background: $primary-color;
         color: #fff;
         box-shadow: $box-shadow;
         z-index: 1;
         position: fixed;
```

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/header/header.component.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/header/header.component.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import { ChangeDetectionStrategy, Component } from "@angular/core";
 import { HeaderService, NavBackService } from "@synerty/peek-plugin-base-js";
 import { LoggedInGuard } from "@peek/peek_core_user";
 import { BehaviorSubject, interval } from "rxjs";
 import { VortexStatusService } from "@synerty/vortexjs";
 import { throttle } from "rxjs/operators";
 import { ThrottleConfig } from "rxjs/internal-compatibility";
+import { DeviceStatusService } from "@peek/peek_core_device";
 
 @Component({
     selector: "header-component",
     templateUrl: "header.component.html",
     styleUrls: ["header.component.scss"],
     changeDetection: ChangeDetectionStrategy.OnPush,
 })
 export class HeaderComponent {
     showSearch$: BehaviorSubject<boolean> = new BehaviorSubject<boolean>(false);
     queuedActionCount$ = new BehaviorSubject<number>(0);
     constructor(
         public headerService: HeaderService,
         private loggedInGuard: LoggedInGuard,
         public navBackService: NavBackService,
-        private vortexStatusService: VortexStatusService
+        private vortexStatusService: VortexStatusService,
+        public deviceStatusService: DeviceStatusService
     ) {
         vortexStatusService.queuedActionCount
             .pipe(
                 throttle(() => interval(800), {
                     leading: false,
                     trailing: true,
                 } as ThrottleConfig)
             )
             .subscribe((queuedActionCount: number) => {
-                console.error(
-                    `HeaderComponent updates queuedActionCount: ${queuedActionCount}`
-                );
                 this.queuedActionCount$.next(queuedActionCount);
             });
     }
 
     get showSearch() {
         return this.showSearch$.getValue();
     }
```

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/status.component.html` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/core/components/status/status.component.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/core/components/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/config/config.page.html` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/config/config.page.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/config/config.page.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/config/config.page.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/home/home.page.scss` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/home/home.page.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/home/home.page.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/home/home.page.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import { ChangeDetectionStrategy, Component } from "@angular/core";
 import { HeaderService, IHeaderLink } from "@synerty/peek-plugin-base-js";
 import { NgLifeCycleEvents, VortexStatusService } from "@synerty/vortexjs";
 import { homeLinks } from "@_peek/plugin-home-links";
 import { BehaviorSubject, interval } from "rxjs";
 import { takeUntil, throttle } from "rxjs/operators";
+import { DeviceStatusService } from "@peek/peek_core_device";
 
 @Component({
     selector: "home-page",
     templateUrl: "home.page.html",
     styleUrls: ["home.page.scss"],
     changeDetection: ChangeDetectionStrategy.OnPush,
 })
 export class HomePage extends NgLifeCycleEvents {
     homeLinks = homeLinks;
     queuedActionCount$ = new BehaviorSubject<number>(0);
     isShowQueuedAction$ = new BehaviorSubject<boolean>(false);
 
     constructor(
         private headerService: HeaderService,
-        private vortexStatusService: VortexStatusService
+        private vortexStatusService: VortexStatusService,
+        public deviceStatusService: DeviceStatusService
     ) {
         super();
         headerService.setTitle("Peek Home");
 
         this.processQueuedActionCount(
             vortexStatusService.snapshot.queuedActionCount
         );
```

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/pages.module.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/pages.module.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts` & `peek-field-app-3.4.0/peek_field_app/src/app/pages/unknown-route/unknown-route.page.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-Medium.ttf` & `peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-Regular.ttf` & `peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/Poppins-SemiBold.ttf` & `peek-field-app-3.4.0/peek_field_app/src/assets/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_docdb/icon.png` & `peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_docdb/icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_search/icon.png` & `peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_search/icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/assets/peek_core_user/plugin_icon.png` & `peek-field-app-3.4.0/peek_field_app/src/assets/peek_core_user/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/favicon.ico` & `peek-field-app-3.4.0/peek_field_app/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/index.html` & `peek-field-app-3.4.0/peek_field_app/src/index.html`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/main.ts` & `peek-field-app-3.4.0/peek_field_app/src/main.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/polyfills.ts` & `peek-field-app-3.4.0/peek_field_app/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/styles/shared.scss` & `peek-field-app-3.4.0/peek_field_app/src/styles/shared.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/styles/styles-layout.scss` & `peek-field-app-3.4.0/peek_field_app/src/styles/styles-layout.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/styles/theme.less` & `peek-field-app-3.4.0/peek_field_app/src/styles/theme.less`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/styles.scss` & `peek-field-app-3.4.0/peek_field_app/src/styles.scss`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/test.ts` & `peek-field-app-3.4.0/peek_field_app/src/test.ts`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app/src/tsconfig.app.json` & `peek-field-app-3.4.0/peek_field_app/src/tsconfig.app.json`

 * *Files identical despite different names*

### Comparing `peek-field-app-3.3.3/peek_field_app.egg-info/SOURCES.txt` & `peek-field-app-3.4.0/peek_field_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 peek_field_app/ios/App/App/Assets.xcassets/AppIcon.appiconset/Contents.json
 peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/Contents.json
 peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-1.png
 peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732-2.png
 peek_field_app/ios/App/App/Assets.xcassets/Splash.imageset/splash-2732x2732.png
 peek_field_app/ios/App/App/Base.lproj/LaunchScreen.storyboard
 peek_field_app/ios/App/App/Base.lproj/Main.storyboard
+peek_field_app/resources/icon.png
 peek_field_app/scripts/build_capacitor_app.sh
 peek_field_app/scripts/exportOptionsPlist.plist.template
 peek_field_app/scripts/prepare_capacitor_ios_app.sh
 peek_field_app/src/_components.scss
 peek_field_app/src/_variables.scss
 peek_field_app/src/favicon.ico
 peek_field_app/src/index.html
```

### Comparing `peek-field-app-3.3.3/setup.py` & `peek-field-app-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_app"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Field UI App."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

