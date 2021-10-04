
***

# Android 6.0 (Marshmallow)

<details>
<summary><p>[Click/tap here to expand/collapse</p>
<p>the dropdown containing the Android Marshmallow logo</p></summary>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/6.0-Marshmallow/Android_Marshmallow_logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/6.0-Marshmallow/Android_Marshmallow_logo.svg)

</details>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/6.0-Marshmallow/Android_6.0-en.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/6.0-Marshmallow/Android_6.0-en.png)

( **Preceeded by:** [Android 5.0 (Lollipop)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-5-0-Lollipop/) | **Succeeded by:** [Android 7.0 (Nougat)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-7-0-Nougat/) )

**Developer:**	Google

**General availability:**	October 2, 2015

**Latest release:**	6.0.1_r81 (MOI10E) / October 1, 2017

**Kernel type:**	Monolithic Kernel (Linux Kernel)

**Official website:**	www.android.com/versions/marshmallow-6-0/

**Support status:** Unsupported

Android Marshmallow (codenamed Android M during development) is the sixth major version of the Android operating system and the 13th version of Android. First released as a beta build on May 28, 2015, it was officially released on October 5, 2015, with the Nexus devices being the first to receive the update.

Marshmallow primarily focuses on improving the overall user experience of its predecessor, Lollipop. It introduced a new permissions architecture, new APIs for contextual assistants (first used by a new feature "Now on Tap" to provide context-sensitive search results), a new power management system that reduces background activity when a device is not being physically handled, native support for fingerprint recognition and USB-C connectors, the ability to migrate data and applications to a microSD card, and other internal changes.

As of August 2021, less than 5% of Android devices use this version, and when it was warned that a billion users use this (or older) version, by then no longer supported with security updates, was when 40% used those versions. Since then at least 70% of the users of those old versions have upgraded to a newer version.

## History

The release was internally codenamed "Macadamia Nut Cookie". The first developer preview build, codenamed Android "M", was unveiled and released at Google I/O on May 28, 2015, for the Nexus 5 and Nexus 6 smartphones, Nexus 9 tablet, and Nexus Player set-top box. The second developer preview was released on July 9, 2015, and the third and final preview was released on August 17, 2015, along with announcing that Android M would be titled Android "Marshmallow".

On September 29, 2015, Google unveiled launch devices for Marshmallow: the LG-produced Nexus 5X, the Huawei-produced Nexus 6P, alongside Google's own Pixel C tablet.

Android 6.0 updates and factory images for Nexus 5, 6, 7 (2013), 9, and Player were released on October 5, 2015. Older Nexus devices, including the Nexus 4, Nexus 7 (2012) and Nexus 10, did not receive an official update.[21] On October 14, 2015, LG announced that it planned to release Marshmallow for its flagship LG G4 smartphone in Poland the following week, marking the first third-party device to receive an update to Marshmallow.

Android 6.0.1, a software patch featuring security fixes, support for Unicode 8.0 emoji (although without supporting skin tone extensions for human emoji), and the return of the "until next alarm" feature in Do Not Disturb mode, was released on December 7, 2015.

## Features

### User experience

A new "Assist" API allows information from a currently opened app, including text and a screenshot of the current screen, to be sent to a designated "assistant" application for analysis and processing. This system is used by the Google Search app feature "Google Now on Tap", which allows users to perform searches within the context of information currently being displayed on-screen. While the "Home" button was used in Android 5 to show available apps, the "Home" button is used now (together with a voice command) to generate on-screen cards which display information, suggestions, and actions related to the content. "Direct Share" allows Share menus to display recently used combinations of contacts and an associated app as direct targets.

### Adoptable storage

The new "Adoptable storage" feature allows a newly-inserted SD card or other secondary storage media to be optionally designated as "internal" rather than "portable" storage.

"Portable" storage is the default behavior used in previous Android versions, treating the media as a secondary storage device for storage of user files, and the storage media can be removed or replaced without repercussions, but user-installed apps are restricted to writing to their respective package name directories located inside Android/data. This restriction was introduced in Android 4.4 KitKat. The Storage Access Framework, through which shared writing access to memory cards has been reinstated in Android 5.0 Lollipop, is backwards-incompatible and slower due to latencies.

When designated as "Internal" storage, the storage media is reformatted with an encrypted ext4 file system, and is "adopted" by the operating system as an extension of the primary storage partition. Existing data (including applications and "private" data folders) are migrated to the external storage, and normal operation of the device becomes dependent on the presence of the media. Apps and operating system functions will not function properly if the adopted storage device is removed, and the card can not be reused in other devices until reformatted. If the user loses access to the storage media, the adopted storage can be "forgotten", which makes the data permanently inaccessible. Samsung and LG have, however, removed the ability to use an SD card as "internal" storage on their Galaxy S7 and G5 devices, with Samsung arguing that the feature could result in unexpected losses of data, and prevents users from being able to transfer data using the card.

### Platform

Android Marshmallow introduces a redesigned application permissions model; apps are no longer automatically granted all of their specified permissions at installation time. An opt-in system is now used, in which users are prompted to grant or deny individual permissions (such as the ability to access the camera or microphone) to an application when they are needed for the first time. Applications remember the grants, which can be revoked by the user at any time. The new permissions model is used only by applications developed for Marshmallow using its software development kit (SDK), and older apps will continue to use the previous all-or-nothing approach. Permissions can still be revoked for those apps, though this might prevent them from working properly, and a warning is displayed to that effect.

Marshmallow introduces new power management schemes known as "Doze" and "App Standby"; when running on battery power, a device will enter a low-power state if it is inactive and not being physically handled. In this state, network connectivity and background processing are restricted, and only "high-priority" notifications are processed. Additionally, network access by apps is deferred if the user has not recently interacted with the app. Apps may request a permission to exempt themselves from these policies, but will be rejected from Google Play Store as a violation of its "Dangerous Products" policy if their core functionality is not "adversely affected" by them.

Android Marshmallow provides native support for fingerprint recognition on supported devices via a standard API, allowing third-party applications to implement fingerprint-based authentication. Fingerprints can be used for unlocking devices and authenticating Play Store and Google Pay purchases. Android Marshmallow supports USB-C, including the ability to instruct devices to charge another device over USB. Marshmallow also introduces "verified links" that can be configured to open directly in their specified application without further user prompts. User data for apps targeting Marshmallow can be automatically backed up to Google Drive over Wi-Fi. Each application receives up to 25 MB of storage, which is separate from a user's Google Drive storage allotment.

As of Marshmallow, the Android Compatibility Definition Document contains new security mandates for devices, dictating that those that are capable of accessing encrypted data without affecting performance must enable secure boot and device encryption by default. These conditions comprise part of a specification that must be met in order to be certified for the operating system, and be able to license Google Mobile Services software. The requirement for mandatory device encryption was originally intended to take effect on Lollipop, but was delayed due to performance issues.

***

## Alternatives

Android 6.x is aging, and it is recommended to use it in a virtual machine via Android x86. However, the devices it runs on are still relevant (as of 2021 October 4th) here are some other alternatives to Android 6.x:

LineageOS

GrapheneOS

ReplicantOS

RemixOS (Android 5.0 and higher)

[Suggest an alternative](https://github.com/seanpm2001/Degoogle-your-life/issues/)

_This article on versions of the Android operating system is a stub. You can help by expanding it._

***

## Sources

[Wikipedia - Android Marshmallow](https://en.wikipedia.org/wiki/Android_Marshmallow/)

Other sources are needed, and this article needs LOTS of improvement and original work to prevent it from being half a copy and paste from Wikipedia.

***

## Article info

**Written on:** `2021 Monday, October 4th at 2:06 pm`

**Last revised on:** `2021 Monday, October 4th at 2:06 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `117`

**Article language:** `English (US) / Markdown`

**Article version:** `1 (2021 Monday, October 4th at 2:06 pm)`

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***
