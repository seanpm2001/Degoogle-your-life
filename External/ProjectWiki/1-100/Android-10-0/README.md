
***

# Android 10.0

<details>
<summary><p>[Click/tap here to expand/collapse</p>
<p>the dropdown containing the Android Q logo</p></summary>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_10_logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_10_logo.svg)

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_Q_Logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_Q_Logo.svg)

</details>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_10_screenshot.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/10.0/Android_10_screenshot.png)

( **Preceeded by:** [Android 9.0 (Pie)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-9-0-Pie/) | **Succeeded by:** [Android 11.0](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-11-0/) )

**Developer:**	Google

**OS family:**	Android

**General availability:**	September 3, 2019;

**Latest release:**	10.0.0_r58 (QSV1.210329.014) / September 8, 2021;

**Kernel type:**	Monolithic Kernel (Linux Kernel)

**Official website:**	[www.android.com/android-10/](https://www.android.com/android-10/)

**Support status:** Supported

Android 10 (codenamed Android Q during development) is the tenth major release and the 17th version of the Android mobile operating system. It was first released as a developer preview on March 13, 2019, and was released publicly on September 3, 2019.

Android 10 was officially released on September 3, 2019 for supported Google Pixel devices, as well as the third-party Essential Phone and Redmi K20 Pro in selected markets. The OnePlus 7T was the first device with Android 10 pre-installed. In October 2019, it was reported that Google's certification requirements for Google Mobile Services will only allow Android 10-based builds to be approved after January 31, 2020.

As of September 2021, 30.04% of Android devices run Android 10 (API 29), making it the second most used version of Android.

## History

Google released the first beta of Android 10 under the preliminary name "Android Q" on March 13, 2019, exclusively on their Pixel phones, including the first-generation Pixel and Pixel XL devices where support was extended due to popular demand. Having been guaranteed updates only up to October 2018, the first-generation Pixel and Pixel XL devices received version updates to Android 10. The Pixel 2 and Pixel 2 XL were included, after being granted an extended warranty period which guaranteed Android version updates for them for at least 3 years from when they were first available on the Google Store. A total of six beta or release-candidate versions were released before the final release.

The beta program was expanded with the release of Beta 3 on May 7, 2019, being made available on 14 partner devices from 11 OEMs; twice as many devices compared to Android Pie's beta. Beta access was removed from the Huawei Mate 20 Pro on May 21, 2019 due to U.S. government sanctions, but was later restored on May 31.

Google released Beta 4 on June 5, 2019 with the finalized Android Q APIs and SDK (API Level 29). Dynamic System Updates (DSU) were also included in Beta 4. The Dynamic System Update allows Android Q devices to temporarily install a Generic System Image (GSI) to try a newer version of Android on top of their current Android version. Once users decide to end testing the chosen GSI image, they can simply reboot their device and boot back into their normal device's Android version.

Google released Beta 5 on July 10, 2019 with the final API 29 SDK as well as the latest optimizations and bug fixes. Google released Beta 6, the final release candidate for testing, on August 7, 2019.

On August 22, 2019, it was announced that Android Q would be branded solely as "Android 10", with no codename. Google ended the practice of giving major releases titles based on desserts, arguing that this was not inclusive to international users (due either to the aforementioned foods not being internationally known, or being difficult to pronounce in some languages). Android VP of engineering Dave Burke did reveal during a podcast that, in addition, most desserts beginning with the letter Q were exotic, and that he personally would have chosen queen cake. He also noted that there were references to "qt"—an abbreviation of quince tart—within internal files and build systems relating to the release.

The statue for the release is likewise the numeral 10, with the Android robot logo (which, as part of an accompanying rebranding, has also been changed to only consist of a head) resting inside the numeral "0".

## Features

### Navigation

Android 10 introduces a revamped full-screen gesture navigation system and new app open and close animations, with gestures such as swiping from either side edge of the display to go back, swiping up to go to the home screen, swiping up and holding to access Overview, swiping diagonally from a bottom corner of the screen to activate the Google Assistant, and swiping along the gesture bar at the bottom of the screen to switch apps. The use of an edge swiping gesture as a "Back" command was noted as potentially causing conflicts with apps that utilize sidebar menus and other functions accessible by swiping. An API can be used by apps to opt out of handling a back gesture within specific areas of the screen, a sensitivity control was added for adjusting the size of the target area to activate the gesture, and Google later stated that the drawer widget would support being "peeked" by long-pressing near the edge of the screen, and then swiped open. The traditional three-key navigation system used since Android "Honeycomb" remains supported as an option, along with the two-button "pill" style navigation introduced in Android 9.0 Pie.

Per Google certification requirements, OEMs are required to support Android 10's default gestures and three-key navigation. OEMs are free to add their own gestures alongside them. However, they must not be enabled by default, they must be listed in a separate area one level deeper than other navigation settings, and they cannot be promoted using notifications. The two-key gesture navigation system used on Android Pie is deprecated, and may not be included on devices that ship with Android 10. However, it can still be included as an option for continuity purposes on devices upgraded from Pie.

### User experience

Android 10 includes a system-level dark mode. Third-party apps can automatically engage a dark mode when it is active.

Apps can also present "settings panels" for specific settings (such as, for example, internet connection and Wi-Fi settings if an app requires internet) via overlay panels, so that the user does not have to be taken outside of the app in order to configure them.
Privacy and security

Several major security and privacy changes are present in Android 10: apps can be restricted by users to only having access to location data when they are actively being used in the foreground. There are also new restrictions on the launching of activities by background apps. For security (due to its use by clickjacking malware) and performance reasons, Android 10 Go Edition forbids use of overlays, except for apps that received the permission before a device was upgraded to Android 10.

### Encryption

In February 2019, Google unveiled Adiantum, an encryption cipher designed primarily for use on devices that do not have hardware-accelerated support for the Advanced Encryption Standard (AES), such as low-end devices. Google stated that this cipher was five times faster than AES-256-XTS on an ARM Cortex-A7 CPU. Therefore, device encryption is now mandatory on all Android 10 devices, regardless of specifications, using Adiantum if their CPU is not capable of hardware-accelerated AES. In addition, implementation of "file-based encryption" (first introduced in Android Nougat) is also mandatory for all devices.

On devices shipping with Android 10, security patches for selected system components (such as ANGLE, Conscrypt, media frameworks, networking components, and others) may be serviced via Google Play Store, without requiring a complete system update ("Project Mainline"). In order to license Google mobile services, manufacturers must support these updates for specific modules, while the remainder are marked as "recommended" but optional. Selected modules within this system use the new APEX package format, a variation of APK files designed for housing and servicing low-level system components.

### Scoped storage

A major change to storage access permissions known as "Scoped storage" is supported on Android 10, and will become mandatory for all apps beginning with Android 11. Apps are only allowed to access files in external storage that they had created themselves (preferably contained within an app-specific directory), and audio, image, and video files contained within the Music, Pictures, or Videos directories. Any other file may only be accessed via user intervention through the backwards-incompatible Google Storage Access Frameworks.

Apps must have a new "read privileged phone state" permission in order to read non-resettable device identifiers, such as IMEI number.
Transport Layer Security

TLS 1.3 support is also enabled by default.

## Platform

Platform optimizations have been made for foldable smartphones, including app continuity when changing modes, changes to multi-window mode to allow all apps to run simultaneously (rather than only the actively-used app running, and all others being considered "paused"), and additional support for multiple displays.

"Direct Share" has been succeeded by "sharing shortcuts". As before, it allows apps to return lists of direct targets for sharing (such as a combination of an app and a specific contact) for use within share menus. Unlike Direct Share, apps publish their targets in advance and do not have to be polled at runtime, improving performance.

Native support has been added for MIDI controllers, the AV1 video codec, the Opus audio codec, and HDR10+. There is also a new standard API for retrieving depth information from camera photos, which can be used for more advanced effects. Native support for aptX Adaptive, LHDC, LLAC, CELT and AAC LATM codecs was added as well.

Android 10 supports WPA3 encryption protocol and Enhanced Open, which introduce opportunistic encryption for Wi-Fi. Android 10 adds support for Dual-SIM dual-standby (DSDS), but is initially only available on the Pixel 3a and Pixel 3a XL.

Android 10 Go Edition has performance improvements, with Google stating that apps would launch 10% quicker than on Pie.

### RISC-V Support

Recently, Android 10 has been ported to the RISC-V architecture by Chinese-owned T-Head Semiconductor. T-Head Semiconductor managed to get Android 10 running on a triple-core, 64-bit, RISC-V CPU of their own design.

***

## Alternatives

Android 10.x is aging, and it is recommended to use it in a virtual machine via Android x86. However, the devices it runs on are still relevant (as of 2021 October 4th) here are some other alternatives to Android 10.x:

LineageOS

GrapheneOS

ReplicantOS

RemixOS (Android 5.0 and higher)

[Suggest an alternative](https://github.com/seanpm2001/Degoogle-your-life/issues/)

_This article on versions of the Android operating system is a stub. You can help by expanding it._

***

## Sources

[Wikipedia - Android 10](https://en.wikipedia.org/wiki/Android_10/)

Other sources are needed, and this article needs LOTS of improvement and original work to prevent it from being half a copy and paste from Wikipedia.

***

## Article info

**Written on:** `2021 Monday, October 4th at 2:59 pm`

**Last revised on:** `2021 Monday, October 4th at 2:59 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `149`

**Article language:** `English (US) / Markdown`

**Article version:** `1 (2021 Monday, October 4th at 2:59 pm)`

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***
