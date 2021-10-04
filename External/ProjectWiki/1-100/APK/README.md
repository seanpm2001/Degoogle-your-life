
***

# Android Package (APK)

**APK Filename extension:**	`.apk`, `.xapk`, `.apks`, `.apkm`

**Internet media type:** `application/vnd.android.package-archive`

**Type of format:**	`Package format`

**Container for Android:** `Mobile apps`

**Container for Windows 11:** `Desktop apps for WSA`

**Extended from:**	`JAR (Java Archive)`

Android Package (APK) is the Android application package file format used by the Android operating system, and a number of other Android-based operating systems for distribution and installation of mobile apps, mobile games and middleware. It can be written in either Java or Kotlin.

APK files can be generated and signed from Android App Bundles.

## Overview

APK is analogous to other software packages such as APPX in Microsoft Windows or a Debian package in Debian-based operating systems. To make an APK file, a program for Android is first compiled using a tool such as Android Studio[3] or Visual Studio and then all of its parts are packaged into one container file. An APK file contains all of a program's code (such as .dex files), resources, assets, certificates, and manifest file. As is the case with many file formats, APK files can have any name needed, but it may be required that the file name ends in the file extension for being recognized as such.

Most Android implementations allow users to manually install APK files only after they turn on an "Unknown Sources" setting that allows installation from sources other than trusted ones like Google Play. One may do so for many reasons, such as during the development of apps, to install apps not found on the store, or to install an older version of an existing app.

## Use on other operating systems

At the Windows 11 announcement event in June 2021, Microsoft showcased the new Windows Subsystem for Android (WSA) that will enable support for the Android Open Source Project (AOSP) and will allow users to run Android apps on their Windows desktop. Microsoft confirmed users will be able to sideload Android apps onto Windows and that it would be possible to install APK files downloaded from third-party sources.

## Package contents

An APK file is an archive that usually contains the following files and directories:

META-INF directory:

MANIFEST.MF: the Manifest file

The certificate of the application.

CERT.SF: The list of resources and a SHA-1 digest of the corresponding lines in the MANIFEST.MF file; for example:

```apk
Signature-Version: 1.0
Created-By: 1.0 (Android)
SHA1-Digest-Manifest: wxqnEAI0UA5nO5QJ8CGMwjkGGWE=
...
Name: res/layout/exchange_component_back_bottom.xml
SHA1-Digest: eACjMjESj7Zkf0cBFTZ0nqWrt7w=
Name: res/drawable-hdpi/icon.png
SHA1-Digest: DGEqylP8W0n0iV/ZzBx3MW0WGCA=
```

lib: the directory containing the compiled code that is platform dependent; the directory is split into more directories within it:

armeabi-v7a: compiled code for all ARMv7 and above based processors only

arm64-v8a: compiled code for all ARMv8 arm64 and above based processors only

x86: compiled code for x86 processors only

x86_64: compiled code for x86-64 processors only

mips and armeabi are Deprecated since NDK r17

res: the directory containing resources not compiled into resources.arsc (see below).

assets: a directory containing applications assets, which can be retrieved by AssetManager.

AndroidManifest.xml: An additional Android manifest file, describing the name, version, access rights, referenced library files for the application. This file may be in Android binary XML that can be converted into human-readable plaintext XML with tools such as AXMLPrinter2, apktool, or Androguard.

classes.dex: The classes compiled in the dex file format understandable by the Dalvik virtual machine and by the Android Runtime.

resources.arsc: a file containing precompiled resources, such as binary XML for example.

***

## Sources

[Wikipedia (EN) - Android Application Package](https://en.wikipedia.org/wiki/Android_application_package)

***

## Article info

**Written on:** `2021 Monday, October 4th at 4:38 pm`

**Last revised on:** `2021 Monday, October 4th at 4:38 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `104`

**Article language:** `English (US)`

**Article version:** `1 (2021 Monday, October 4th at 4:38 pm)`

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***
