
***

# Stagefright (bug)

_Not to be confused with the stagefright library for Android._

![https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Stagefright(bug)/Stagefright_bug_logo.png](https://github.com/seanpm2001/Degoogle-your-life/blob/main/Graphics/Stagefright(bug)/Stagefright_bug_logo.png)

_Logo of the Stagefright library bug_

**CVE identifier(s)**	`CVE-2015-1538`, `CVE-2015-1539`, `CVE-2015-3824`, `CVE-2015-3826`, `CVE-2015-3827`, `CVE-2015-3828`, `CVE-2015-3829`, `CVE-2015-3864` (Stagefright 1.0), `CVE-2015-6602` (Stagefright 2.0)

**Date discovered:**	`27 July 2015`;

**Date patched:**	`3 August 2015`;

**Discoverer:**	`Joshua Drake (Zimperium)`

**Affected software:**	`Android 2.2 "Froyo"` and later (Stagefright 1.0), `Android 1.5 "Cupcake"` to `Android 5.1 "Lollipop"` (Stagefright 2.0)

Stagefright is the name given to a group of software bugs that affect versions 2.2 "Froyo" of the Android operating system. The name is taken from the affected library, which among other things, is used to unpack MMS messages. Exploitation of the bug allows an attacker to perform arbitrary operations on the victim's device through remote code execution and privilege escalation. Security researchers demonstrate the bugs with a proof of concept that sends specially crafted MMS messages to the victim device and in most cases requires no end-user actions upon message reception to succeed—the user doesn't have to do anything to 'accept' exploits using the bug; it happens in the background. A phone number is the only information needed to carry out the attack.

The underlying attack vector exploits certain integer overflow vulnerabilities in the Android core component called libstagefright, which is a complex software library implemented primarily in C++ as part of the Android Open Source Project (AOSP) and used as a backend engine for playing various multimedia formats such as MP4 files.

The discovered bugs have been provided with multiple Common Vulnerabilities and Exposures (CVE) identifiers, CVE-2015-1538, CVE-2015-1539, CVE-2015-3824, CVE-2015-3826, CVE-2015-3827, CVE-2015-3828, CVE-2015-3829 and CVE-2015-3864 (the latter one has been assigned separately from the others), which are collectively referred to as the Stagefright bug.

## History

The Stagefright bug was discovered by Joshua Drake from the Zimperium security firm, and was publicly announced for the first time on July 27, 2015. Prior to the announcement, Drake reported the bug to Google in April 2015, which incorporated a related bugfix into its internal source code repositories two days after the report. In July 2015, Evgeny Legerov, a Moscow-based security researcher, announced that he had found at least two similar heap overflow zero-day vulnerabilities in the Stagefright library, claiming at the same time that the library has been already exploited for a while. Legerov also confirmed that the vulnerabilities he discovered become unexploitable by applying the patches Drake submitted to Google.

The public full disclosure of the Stagefright bug, presented by Drake, took place on August 5, 2015 at the Black Hat USA computer security conference, and on August 7, 2015 at the DEF CON 23 hacker convention. Following the disclosure, on August 5, 2015, Zimperium publicly released the source code of a proof-of-concept exploit, actual patches for the Stagefright library (although the patches were already publicly available since early May 2015 in the AOSP and other open-source repositories), and an Android application called "Stagefright detector" that tests whether an Android device is vulnerable to the Stagefright bug.

As of August 3, 2015, only a few products have been actually patched against the bug: Blackphone's PrivatOS since its version 117, nightly releases of the CyanogenMod 12.0 and 12.1, Sprint's variant of the Samsung Galaxy Note 4, the Moto E, G, and X, Droid Maxx, Mini, and Turbo, and Mozilla Firefox since its version 38 (and Firefox OS since 2.2) (this web browser internally uses Android's Stagefright library).

On August 13, 2015, another Stagefright vulnerability, CVE-2015-3864, was published by Exodus Intelligence. This vulnerability was not mitigated by existing fixes of already known vulnerabilities. CyanogenMod team published a notice that patches for CVE-2015-3864 have been incorporated in CyanogenMod 12.1 source on August 13, 2015.

On October 1, 2015, Zimperium released details of further vulnerabilities, also known as Stagefright 2.0. This vulnerability affects specially crafted MP3 and MP4 files that execute their payload when played using the Android Media server. The vulnerability has been assigned identifier CVE-2015-6602 and was found in a core Android library called libutils; a component of Android that has existed since Android was first released. Android 1.5 through 5.1 are vulnerable to this new attack and it is estimated that one billion devices are affected.

## Implications

While Google maintains the Android's primary codebase and firmware, updates for various Android devices are the responsibility of wireless carriers and original equipment manufacturers (OEMs). As a result, propagating patches to the actual devices often introduces long delays due to a large fragmentation between the manufacturers, device variants, Android versions, and various Android customizations performed by the manufacturers; furthermore, many older or lower cost devices may never receive patched firmware at all. Many of the unmaintained devices would need to be rooted, which violates the terms of many wireless contracts. Therefore, the nature of Stagefright bug highlights the technical and organizational difficulties associated with the propagation of Android patches.

As an attempt to address the delays and issues associated with the propagation of Android patches, on August 1, 2015 Zimperium formed the Zimperium Handset Alliance (ZHA) as an association of different parties interested in exchanging information and receiving timely updates on Android's security-related issues. Members of the ZHA also received source code of the Zimperium's proof-of-concept Stagefright exploit before it was publicly released. As of August 6, 2015, 25 of the largest Android device OEMs and wireless carriers have joined the ZHA.

## Mitigation

Certain mitigations of the Stagefright bug exist for devices that run unpatched versions of Android, including disabling the automatic retrieval of MMS messages and blocking the reception of text messages from unknown senders. However, these two mitigations are not supported in all MMS applications (the Google Hangouts app, for example, only supports the former), and they do not cover all feasible attack vectors that make exploitation of the Stagefright bug possible by other means, such as by opening or downloading a malicious multimedia file using the device's web browser.

At first it was thought that further mitigation could come from the address space layout randomization (ASLR) feature that was introduced in Android 4.0 "Ice Cream Sandwich", fully enabled in Android 4.1 "Jelly Bean"; The version of Android 5.1 "Lollipop" includes patches against the Stagefright bug. Unfortunately, later results and exploits like Metaphor that bypass ASLR were discovered in 2016.

As of Android 10, software codecs were moved to a constrained sandbox which effectively mitigates this threat for devices capable of running this version of the OS.

***

## Sources

[Wikipedia (EN) - Stagefright (bug)](https://en.wikipedia.org/wiki/Stagefright_(bug))

***

## Article info

**Written on:** `2021 Monday, October 4th at 4:47 pm`

**Last revised on:** `2021 Monday, October 4th at 4:47 pm`

**File format** `Markdown document (*.md *.mkd *.markdown)`

**Line count (including blank lines and compiler line):** `81`

**Article language:** `English (US)`

**Article version:** `1 (2021 Monday, October 4th at 4:47 pm)`

**All times are UTC-7 (PDT/Pacific Time)**

**You may need special rendering support for the `<dropdown>` HTML tag being used in this document**

***
