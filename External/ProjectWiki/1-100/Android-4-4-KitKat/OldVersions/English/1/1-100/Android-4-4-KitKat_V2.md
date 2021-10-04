
***

# Android 4.4 (KitKat)

<details>
<summary><p>[Click/tap here to expand/collapse</p>
<p>the dropdown containing the Android KitKat logo</p></summary>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/4.4-KitKat/Android_KitKat_logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/4.4-KitKat/Android_KitKat_logo.svg)

</details>

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/4.4-KitKat/Nexus_5_(Android_4.4.2)_Screenshot.jpg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Android/Versions/4.4-KitKat/Nexus_5_(Android_4.4.2)_Screenshot.jpg)

( **Preceeded by:** [Android 4.1 (Jelly Bean)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-4-1-Jelly-Bean/) | **Succeeded by:** [Android 5.0 (Lollipop)](https://github.com/seanpm2001/Degoogle-your-life/wiki/Android-5-0-Lollipop/) )

**Developer:**	Google

**Released to manufacturing:**	October 31, 2013;

**Latest release:**	4.4.4_r2.0.1 (KTU84Q) / July 7, 2014;

**Kernel type:**	Monolithic Kernel (Linux Kernel)

**Official website:**	[www.android.com/versions/kit-kat-4-4/](https://www.android.com/versions/kit-kat-4-4/)

**Support status:** Unsupported

Android KitKat is the codename for the eleventh Android mobile operating system, representing release version 4.4. Unveiled on September 3, 2013, KitKat focused primarily on optimizing the operating system for improved performance on entry-level devices with limited resources.

As of October 2020, 1.47% of Android devices run KitKat.

## History

Android 4.4 "KitKat" was officially announced on September 3, 2013. The release was internally codenamed "Key lime pie"; John Lagerling, director of Android global partnerships, and his team, decided to drop the name, arguing that "very few people actually know the taste of a key lime pie". Aiming for a codename that was "fun and unexpected", his team pursued the possibility of naming the release "KitKat" instead. Lagerling phoned a representative of Nestlé, who owns the Kit Kat brand and produces the confectionary (outside the United States, where it is produced by The Hershey Company under license), and quickly reached a preliminary deal for a promotional collaboration between the two companies, later finalized in a meeting at Mobile World Congress in February 2013. The partnership was not revealed publicly, or even to other Google employees and Android developers (who otherwise continued to internally refer to the OS as "KLP"), until its official announcement in September.

As part of the promotional efforts, Kit Kat bars in the shape of the Android robot logo were produced, while Hershey ran a contest in the United States with prizes of Nexus 7 tablets and Google Play Store credit.

The Nexus 5, developed by LG Electronics, was unveiled on September 30, 2013, as the launch device for KitKat.

Up to October 2017, Android 4.4 was still supported with security patches by Google for the source code.

## Development

Continuing on from the focus on improving visual performance and responsiveness on Android 4.1 "Jelly Bean", the main objective of Android 4.4 was to optimize the platform for better performance on low-end devices, without compromising its overall capabilities and functionality. The initiative was codenamed "Project Svelte", which Android head of engineering Dave Burke joked was a weight loss plan after Jelly Bean's "Project Butter" added "weight" to the OS.[ To simulate lower-spec devices, Android developers used Nexus 4 devices underclocked to run at a reduced CPU speed with only a single core active, 512 MB memory, and at 960×540 display resolution—specifications meant to represent a common low-end Android device.

A development tool known as ProcStats was developed in order to analyze the memory usage of apps over time, especially those that run background services. This data was used to optimize and decouple Google apps and services found to be inefficient, thus helping to reduce the overall memory usage of Android. Additionally, 4.4 was designed to be more aggressive in managing memory, helping to guard against apps wasting too much memory.

## Features

### User experience

The overall interface of KitKat further downplays the "Holo" interface appearance introduced on 4.0, replacing remaining instances of blue accenting with greys and white (such as the status bar icons), and getting rid of the Wi-Fi upstream and downstream traffic indicators (triangles pointing up and down), though they can still be seen in the quick control center menu.

The Wi-Fi icon colour when only a connection to an access point with no Internet access has been established has changed from grey to orange.

The appearance may deviate in custom vendor distributions such as TouchWiz.

Apps may trigger a translucent status and navigation bar appearance, or trigger a full screen mode ("Immersive mode") to hide them entirely. The launcher also received a refreshed appearance, with the implementation of the translucent navigation bars, and the replacement of the black backdrop in the application drawer with a translucent backdrop. Additionally, action overflow menu buttons in apps are always visible, even on devices with the deprecated "Menu" navigation key. In the Settings menu, users can now specify a default Home (launcher) and text messaging app.

On stock devices, the Messaging and Movie Studio apps were removed; the former was replaced by Google Hangouts, which supported SMS. The AOSP Gallery app was also deprecated in favor of Google+ Photos.

### Platform

A new runtime environment known as the Android Runtime (ART), intended to replace the Dalvik virtual machine, was introduced as a technology preview in KitKat. ART is a cross-platform runtime which supports the x86, ARM, and MIPS architectures in both 32-bit and 64-bit environments. Unlike Dalvik, which uses just-in-time compilation (JIT), ART compiles apps upon installation, which are then run exclusively from the compiled version from then on. This technique removes the processing overhead associated with the JIT process, improving system performance.

Devices with 512 MB of RAM or less report as "low RAM" devices. Using an API, apps may detect low RAM devices and modify their functionality accordingly. KitKat also supports zram. WebView components were updated to utilize a version of the Google Chrome rendering engine. A new Storage Access Framework API allows apps to retrieve files in a consistent manner; as part of the framework, a new system file picker (branded as "Documents") allows users to access files from various sources (including those exposed by apps, such as online storage services).

A public API was introduced for creating and managing text messaging clients. Sensor batching, step detection and counter APIs were also added. KitKat supports host card emulation for near-field communications, which allows apps to emulate a smart card for activities such as mobile payments.

## Criticism

### Memory card writing disabled

Writing access to MicroSD memory cards for non-system (user-installed) software has been disabled in this Android version, with no official option to manually grant selected applications write access.

As a response, many users proceeded to root their devices to circumvent the restriction.

The restriction was officially lifted in Android 5.0 Lollipop, albeit only for applications with an updated API level (≥20), restricting backwards compatibility.

Writing access on the internal storage and USB On-The-Go was unaffected by the restriction yet.

#### Notes

One directory exempt from this restriction is each application's own dedicated user data folder, located inside the Android/data/ directory on the memory card, with the application's package name.

## Alternatives

Android 4.4 is aging, and it is recommended to use it in a virtual machine via Android x86. However, the devices it runs on are still relevant (as of 2021 October 4th) here are some other alternatives to Android 4.4:

LineageOS

GrapheneOS

ReplicantOS

[Suggest an alternative](https://github.com/seanpm2001/Degoogle-your-life/issues/)

<!-- RemixOS (Android 5.0 and higher) !-->

_This article on versions of the Android operating system is a stub. You can help by expanding it._

***

## Sources

[Wikipedia - Android KitKat](https://en.wikipedia.org/wiki/Android_KitKat)

Other sources are needed, and this article needs LOTS of improvement and original work to prevent it from being half a copy and paste from Wikipedia.

***

## Article info

**Written on:** `2021 Monday, October 4th at 1:26 pm`

**Last revised on:** `2021 Monday, October 4th at 1:35 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `133`

**Article language:** `English (US)`

**Article version:** `2 (2021 Monday, October 4th at 1:35 pm)` V2: Added the predecessor and successor section, as it was not added originally.

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***
