
***

# ChromiumOS

_This article is on the open source web browser "operating system" by Google. For the open source browser, see [Chromium](https://github.com/seanpm2001/Degoogle-your-life/wiki/Google-Chromium/) for the proprietary web browser for cheap laptops, see [ChromeOS](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeOS/) for the proprietary web browser, see [Google Chrome](https://github.com/seanpm2001/Degoogle-your-life/wiki/Google-Chrome/) for ChromeOS hardware, see ( [Chromebook](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromebook/), [Chromebase](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromebase/), [Chromebox](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeBox/), [Chromeblet](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromeblet/), [Chromebit](https://github.com/seanpm2001/Degoogle-your-life/wiki/ChromeBit/) ) for the device casting service, see [Chromecast](https://github.com/seanpm2001/Degoogle-your-life/wiki/Chromecast/)_

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Logo/Chromium_logo_with_wordmark.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Logo/Chromium_logo_with_wordmark.png)

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Browser/ChromiumOS-desk.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Browser/ChromiumOS-desk.png)

_Chromium OS (85.0.4163.0 ) displaying the New Tab Page_

**Developer:**	`Google`

**OS family:**	`Linux`

**Working state:**	`Current`

**Source model:**	`Open source`

**Repository:** [chromium.googlesource.com/chromiumos/](chromium.googlesource.com/chromiumos/)

**Update method:**	`Rolling release`

**Platforms:**	`x86`, `x64`, `ARM`, `ARM64`

**Kernel type:**	`Monolithic (Linux kernel)`

**Userland:**	`Ozone (Display manager), X11, GNU`

**Default user interface:**	`Chromium, Aura Shell (Ash)`

**License:**	`Various open source licenses (mainly BSD-style licenses and GPL)`

**Official website:** [www.chromium.org/chromium-os](www.chromium.org/chromium-os)

Chromium OS is a free and open-source operating system designed for running web applications and browsing the World Wide Web. It is the open-source version of Chrome OS, a Linux distribution made by Google.

Like Chrome OS, Chromium OS is based on the Linux kernel, but its principal user interface is the Chromium web browser rather than the Google Chrome browser. Chromium OS also includes the Portage package manager, which was originally developed for Gentoo Linux. Because Chromium OS and Chrome OS use a web browser engine for the user interface, they are oriented toward web applications rather than desktop applications or mobile apps.

Google first published the Chromium OS source code in late 2009.

## Architecture

Chromium's architecture is three-tiered, consisting of "three major components":

The Chromium-based browser and the window manager

System-level software and user-land services: the Linux kernel, drivers, connection manager, and so on

Firmware

## Availability

Chromium OS was first made available in compiled form by hobbyists. More organized efforts have emerged over time, including a few manufacturers that have shipped devices with the operating system pre-installed.

## Builds and forks

By May 2010, compiled versions of the work-in-progress source code had been downloaded from the Internet more than a million times. The most popular version, entitled "Chromium OS Flow", was created by Liam McLoughlin, a then 17-year-old college student in Liverpool, England, posting under the name "Hexxeh". McLoughlin's build boots from a USB memory stick and included features that Google engineers had not yet implemented, such as support for the Java programming language. While Google did not expect that hobbyists would use and evaluate Chromium OS ahead of its official release, Sundar Pichai, Google's vice president of product management (now the CEO) said that "what people like Hexxeh are doing is amazing to see." Pichai said the early releases were an unintended consequence of open source development. "If you decide to do open-source projects, you have to be open all the way."

Hexxeh's work continued into the following year. He announced "Chromium OS Lime" in December 2010, and in January 2011, released "Luigi", an application designed to "jailbreak"/"root" the Google Cr-48 "Mario" prototype hardware and install a generic BIOS. The developer made the builds available in virtual machine format on March 13, 2011. With no official build of Chromium OS forthcoming from Google, Hexxeh's "vanilla" nightly builds of Chromium OS were the principal resource for people wanting to try Chromium OS. Hexxeh stopped uploading his builds on April 20, 2013.

More recent versions of Chromium OS are available from Arnoldthebat, who maintains daily and weekly builds] along with usage guidelines and help. In July 2012, Chromium Build Kit was released. It automatically compiles a developer build and installs Chromium OS on a USB drive.

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Cherry_-_on_web.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Cherry_-_on_web.png)

ChromiumOS Cherry

Now known as "Flow"

(4 December 2009)

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Zero_-_login_screen.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Zero_-_login_screen.png)

ChromiumOS Zero

Now known as "Vanilla "

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Flow_-_login_screen.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/ChromiumOS/Startup/Splash/ChromiumOS_Flow_-_login_screen.png)

(9 December 2009)

ChromiumOS Flow

(15 February 2010)

In 2015, New York City-based Neverware produced a Chromium OS fork called CloudReady aimed at the educational market, with the intention of extending the life of older PCs and laptops. A subsequent version can dual-boot Neverware and the Windows operating system (until v64).

In 2016, Nexedi released NayuOS, a fork of Chromium OS precompiled for several Chromebook computers. The operating system provides Chrome OS-like capabilities without storing data on Google servers. It optionally removes the Google login and provides additional developer tools.

Also in 2016, a London/Beijing-based startup produced a line of Chromium OS fork named Flint OS, targeting a wider range of platforms, including 64-bit PCs, Raspberry Pi, Tinker Board, Firefly development boards, and VMware virtual machines. The OS was later renamed Fyde OS

## Hardware

Some devices have shipped with Chromium OS preinstalled. In May 2011, Dell also released a new build for the Dell Inspiron Mini 10v netbook, following up on an earlier build released almost 18 months earlier. The build did not support audio, but was bootable from a USB drive. Other devices include the Kogan Agora Chromium Laptop by the Australian company Kogan and the Xi3 Modular Computer, introduced by the company of the same name. In late 2015, a team headed by Dylan Callahan released a beta Chromium OS port to the Raspberry Pi 2 single-board computer. In 2016, Flint Innovations released a Chromium OS port for the latest Raspberry Pi 3/B model named Flint OS for RPi. Subsequently, this project has been fully open-sourced at GitHub, with all the files and detailed instructions to re-create the build.

## Trademark dispute

In June 2011, ISYS Technologies, based in Salt Lake City, sued Google in a Utah district court, claiming rights to the name "Chromium" and, by default, Chromebook and Chromebox. The suit sought to stop Google and its hardware and marketing partners from selling Chromebooks. The suit was later dismissed and, as part of an undisclosed settlement between Google and ISYS, ISYS abandoned its trademark efforts.


## Sources

[Wikipedia - ChromiumOS](https://en.wikipedia.org/wiki/Chromium_OS)

Other sources are needed, and this article needs LOTS of improvement and original work to prevent it from being a copy and paste from Wikipedia.

***

## Article info

**Written on:** `2021 Tuesday, October 5th at 4:30 pm`

**Last revised on:** `2021 Tuesday, October 5th at 4:30 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Article version:** `1 (2021 Tuesday, October 5th at 4:30 pm)`

**Article language:** `English (US) / Markdown`

**Line count (including blank lines and compiler line):** `138`

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***

<!-- Tools

Quick copy and paste

https://github.com/seanpm2001/WacOS/wiki/

!-->
