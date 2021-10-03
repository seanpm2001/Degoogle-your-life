
***

# Google Chromium

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2014/Chromium_Material_Icon.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2014/Chromium_Material_Icon.svg)

This article is on the open source web browser by Google. For the proprietary browser, see [Google Chrome](https://github.com/seanpm2001/Degoogle-your-life/wiki/Google-Chrome/) for the proprietary web browser for cheap laptops, see [ChromeOS](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeOS/) for the development channel of ChromeOS that is open source, see [ChromiumOS](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromiumOS/) for ChromeOS hardware, see ( [Chromebook](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromebook/), [Chromebase](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromebase/), [Chromebox](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeBox/), [Chromeblet](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromeblet/), [Chromebit](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeBit/) ) for the device casting service, see [Chromecast](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromecast/)

Chromium is a free and open-source codebase for a web browser, principally developed and maintained by Google. Google uses the code to make its Chrome web browser, which has additional features.

The Chromium codebase is widely used. Microsoft Edge, Opera, and many other browsers are based on the code. Other parties compile it and release browsers with the Chromium name and logo. Moreover, significant portions of the code are used by several app frameworks.

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Linux/Ubuntu/Chromium_78_running_on_GNOME_Shell_and_Ubuntu_Linux.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Linux/Ubuntu/Chromium_78_running_on_GNOME_Shell_and_Ubuntu_Linux.png)

Chromium's user interface is minimalist, as one of Google's initial goals was to make the browser "feel lightweight (cognitively and physically) and fast".

## Licensing

Chromium is an entirely free and open-source software project. The Google-authored portion is shared under the 3-clause BSD license. Other parts are subject to a variety of licenses, including MIT, LGPL, Ms-PL, and an MPL/GPL/LGPL tri-license.

This licensing permits any party to build the codebase and share the resulting browser executable with the Chromium name and logo. Thus many Linux distributions do this, as well as FreeBSD and OpenBSD.

## Differences from Google Chrome

Chromium provides the vast majority of source code for Google Chrome, so the name "Chromium" was chosen by Google because chromium metal is used in chrome plating.

There is no Chromium build from Google. All browsers released with the Chromium name and logo are built by other parties.

## Features

Chromium lacks the following Chrome features:

Automatic browser updates

API keys for some Google services, including browser sync

The Widevine DRM module

Licensed codecs for the popular H.264 video and AAC audio formats

Tracking mechanisms for usage and crash reports

## Branding and licensing

While Chrome has the same user interface functionality as Chromium, it changes the color scheme to the Google-branded one. Unlike Chromium, Chrome is not open-source, so its binaries are licensed as freeware under the Google Chrome Terms of Service.

## Development

The Chromium browser codebase contains about 35 million source lines of code.

## Contributors

Chromium has been a Google project since its inception, and Google employees have done the bulk of the development work.

Google refers to this project and the offshoot Chromium OS as "The Chromium Projects", and its employees use @chromium.org email addresses for this development work. However, in terms of governance, "Chromium Projects" are not independent entities; Google retains firm control of them.

The Chromium browser codebase is widely used, so others have made important contributions, most notably Microsoft, Igalia, Yandex, Intel, Samsung, LG, Opera, and Brave Some employees of these companies also have @chromium.org email addresses.

## Programming languages

C++ is the primary language, comprising about half of the codebase. This includes the Blink and V8 engines, the implementation of HTTP and other protocols, the internal caching system, and other essential browser components.

Some of the user interface is implemented in HTML, CSS, and JavaScript. An extensive collection of web platform tests are also written in these languages.

About 10% of the codebase is written in C. This is mostly from third-party libraries that provide essential functionality, such as SQLite and numerous codecs.

Support for mobile operating systems requires special languages: Java for Android, and for iOS both Swift and Objective-C. (A copy of Apple's WebKit engine is also in the codebase, since it is required for iOS browsers.)

## Logistics

The bug tracking system is a publicly accessible website. Participants are identified by their email addresses.

The Chromium continuous integration system automatically builds and tests the codebase several times a day.

Builds are identified by a four-part version number that is major.minor.build.patch. This versioning scheme and the branch points that occur every six to seven weeks are from Google Chrome and its development cycle.

## History

### 2008 to 2010

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2008/Google-Chromium-first-logo.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2008/Google-Chromium-first-logo.png)

Google Chrome debuted in September 2008, and along with its release, the Chromium source code was also made available, allowing builds to be constructed from it.

Upon release, Chrome was criticized for storing a user's passwords without the protection of a master password. Google has insisted that a master password provides no real security against knowledgeable hackers, but users argued that it would protect against co-workers or family members borrowing a computer and being able to view stored passwords as plaintext. In December 2009, Chromium developer P. Kasting stated: "A master password was issue 1397. That issue is closed. We will not implement a master password. Not now, not ever. Arguing for it won't make it happen. 'A bunch of people would like it' won't make it happen. Our design decisions are not democratic. You cannot always have what you want."

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Linux/Splash/File-Chromium-Linux-Alpha.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Linux/Splash/File-Chromium-Linux-Alpha.png)

_An alpha build of Chromium 3 for Linux_

Version 3 was the first alpha available for Linux. Chromium soon incorporated native theming for Linux, using the GTK+ toolkit to allow it fit into the GNOME desktop environment. Version 3 also introduced JavaScript engine optimizations and user-selectable themes.

Version 6 introduced features for user interface minimalism, including a unified single page and tools menu, no home button by default (although user configurable), a combined reload/stop button, bookmark bar deactivated by default. It also introduced an integrated PDF reader, WebM and VP8 support for use with HTML5 video, and a smarter URL bar.

Version 7 boosted HTML5 performance to twice that of prior versions via hardware acceleration.

Version 8 focused on improved integration into Chrome OS and improved cloud features. These include background web applications, host remoting (allowing users centrally to control features and settings on other computers) and cloud printing.

Version 9 introduced a URL bar feature for exposing phishing attacks, plus sandboxing for the Adobe Flash plug-in. Other additions were the WebGL library and access for the new Chrome Web Store.

### 2011

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2011/Chromium_11_Logo.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2011/Chromium_11_Logo.svg)

_Chromium logo introduced in 2011_

In February, Google announced that it was considering large-scale user interface (UI) changes, including at least partial elimination of the URL bar, which had been a mainstay of browsers since the early years of the Web. The proposed UI was to be a consolidation of the row of tabs and the row of navigation buttons, the menu, and URL bar into a single row. The justification was freeing up more screen space for web page content. Google acknowledged that this would result in URLs not always being visible to the user, that navigation controls and menus may lose their context, and that the resulting single line could be quite crowded. However, by August, Google decided that these changes were too risky and shelved the idea.

In March, Google announced other directions for the project. Development priorities focused on reducing the size of the executable, integrating web applications and plug-ins, cloud computing, and touch interface support. Thus a multi-profile button was introduced to the UI, allowing users to log into multiple Google and other accounts in the same browser instance. Other additions were malware detection and support for hardware-accelerated CSS transforms.

By May, the results of Google's attempts to reduce the file size of Chromium were already being noted. Much of the early work in this area concentrated on shrinking the size of WebKit, the image resizer, and the Android build system. Subsequent work introduced a more compact mobile version that reduced the vertical space of the UI.

Other changes in 2011 were GPU acceleration on all pages, adding support for the new Web Audio API, and the Google Native Client (NaCl) which permits native code supplied by third parties as platform-neutral binaries to be securely executed within the browser itself. Google's Skia graphics library was also made available for all Chromium versions.

### Since 2012

The sync service added for Google Chrome in 2012 could also be used by Chromium builds. The same year, a new API for high-quality video and audio communication was added, enabling web applications to access the user's webcam and microphone after asking permission to do so. Then GPU accelerated video decoding for Windows and support for the QUIC protocol were added.

In 2013, Chromium's modified WebKit rendering engine was officially forked as the Blink engine.

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2014/Chromium_Material_Icon.svg](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Google-Chromium/Logo/2014/Chromium_Material_Icon.svg)

In 2014, the logo was changed again.

Other changes in 2013 were the ability to reset user profiles and new browser extension APIs Tab indicators for audio and webcam usage were also added, as was automatic blocking of files detected as malware.

Version 69 introduced a new browser theme, as part of the 10th anniversary of Google Chrome. The same year, new measures were added to curtail abusive advertising.

Starting in March 2021, the Google Chrome sync service can no longer be used by Chromium builds.

### Browsers based on Chromium

In addition to Google Chrome, many other notable web browsers have been based on the Chromium code.

### Active

Amazon Silk

Avast Secure Browser developed by Avast

Beaker, a peer-to-peer web browser

Blisk is a browser available for Windows 7 and later, OS X 10.9 and later that aims to provide an array of useful tools for Web development.

Brave is an open-source web browser that aims to block website trackers and remove intrusive internet advertisements.

CodeWeavers CrossOver Chromium is an unofficial bundle of a Wine derivative and Chromium Developer Build 21 for Linux and macOS, first released on 15 September 2008 by CodeWeavers as part of their CrossOver project.

Comodo Dragon is a rebranded version of Chromium for 32-bit Windows 8.1, 8, Windows 7 and Vista produced by the Comodo Group. According to the developer, it provides improved security and privacy features.

Cốc Cốc is a freeware web browser focused on the Vietnamese market, developed by Vietnamese company Cốc Cốc, based on Chromium open-source code for Windows. According to data published by StatCounter in July 2013, Cốc Cốc has passed Opera to become one of the top 5 most popular browsers in Vietnam within 2 months after its official release.

Dissenter is a fork of Brave browser that adds a comment section to any URL.

Epic Browser is a privacy-centric web browser developed by Hidden Reflex of India and based on Chromium source code

Falkon an open-source Qt-based GUI, using the Chromium-based QtWebEngine.

qutebrowser a Qt-based GUI with Vim-like keybindings, using the Chromium-based QtWebEngine.

Microsoft Edge is Chromium-based as of 15 January 2020.

Naver Whale is a South Korean freeware web browser developed by Naver Corporation, which is also available in English. It became available on Android on 13 April 2018.

Opera began to base its web browser on Chromium with version 15.

Qihoo 360 Secure Browser is a Chromium-based Chinese web browser developed by Qihoo.

SalamWeb is a web browser based on Chromium for Muslims, which only allows Halal websites/information.

Samsung Internet shipped its first Chromium-based browser in a Galaxy S4 model released in 2013.

Sleipnir is a Chromium derivative browser for Windows and macOS. One of its main features is linking to Web apps (Facebook, Twitter, Dropbox, etc.) and smartphone apps (Google Map, etc.). It also boasts what it calls "beautiful text," and has unique graphical tabs, among other features.

Slimjet: A Chromium-based web browser released by FlashPeak that features built-in webpage translation, PDF viewing capability and a PPAPI flash plugin, features usually missing from Chromium-based browsers currently not supported.

SRWare Iron is a freeware release of Chromium for Windows, macOS and Linux, offering both installable and portable versions. Iron disables certain configurable Chromium features that could share information with third parties and additional tracking features that Google adds to its Chrome browser.

Torch is a browser based on Chromium for Windows. It specialises in media downloading and has built-in media features, including a torrent engine, video grabber and sharing button.

ungoogled-chromium is a browser based on Chromium. Initially developed for Linux, versions for Windows and MacOS were later added. It removes Google services built into Chromium.

Vivaldi is a browser for Windows, macOS and Linux developed by Vivaldi Technologies. Chromium-based Vivaldi aims to revive the rich features of the Presto-era Opera with its own proprietary modifications.

Yandex Browser is a browser created by the Russian software company Yandex for macOS, Windows, Linux, Android and iOS. The browser integrates Yandex services, which include a search engine, a machine translation service and cloud storage. On Android it provides ability to install chrome extensions on a mobile browser.

### Discontinued

Flock – a browser that specialized in providing social networking and had Web 2.0 facilities built into its user interface. It was based on Chromium starting with version 3.0. Flock was discontinued in April 2011.

Redcore – a browser developed by Chinese company Redcore Times (Beijing) Technology Ltd. and marketed as a domestic product that was developed in-house, but was revealed to be based on Chromium

Rockmelt – a Chromium-based browser for Windows, macOS, Android and iOS under a commercial proprietary licence. It integrated features from Facebook and Twitter, but was discontinued in April 2013 and fully retired at 10am PT on 31 July 2013. On 2 August 2013, Rockmelt was acquired by Yahoo! Rockmelt's extensions and its website was shut down after 31 August 2013. Yahoo! plans to integrate Rockmelt's technology into other products.

## Use in app frameworks

Significant portions of the Chromium code are used by some application frameworks. Notable examples are Electron, the Chromium Embedded Framework, and the Qt WebEngine. These frameworks have been used to create many apps.

## Alternatives

It is very easy to alternate from Google Chrome. Here are some of the common browsers people switch to:

Mozilla Firefox

> Waterfox

> TenFourFox (Firefox for Mac OS X 10.0 to 10.4)

Pale Moon

SeaMonkey

Tor

Brave

Microsoft Edge

Safari

DuckDuckGo (browser)

Samsung Internet

Opera

> Opera GX

> Opera Mini

> Opera mobile

_This list is incomplete._

Not all these alternates are good for privacy however.

***

## Sources

[Chromium (web browser) on Wikipedia](https://en.wikipedia.org/wiki/Chromium_(web_browser))

I need more sources and better sources for this article. This article also needs to be rewritten, as it is a copy and paste from Wikipedia.

***

## Article info

**Written on:** `2021 Saturday, October 2nd at 6:54 pm`

**Last revised on:** `2021 Saturday, October 2nd at 6:54 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `269`

**Article version:** `1 (2021 Saturday, October 2nd at 6:54 pm)`

***

<!-- Tools

Quick copy and paste

https://github.com/seanpm2001/Degoogle-your-life/wiki/

!-->
