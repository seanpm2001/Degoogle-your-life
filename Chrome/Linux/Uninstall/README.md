
***

# Removing Chrome from Linux

By default, some Linux distributions come with Google Chrome and or Google Chromium pre-installed. Notable Linux distributions that do this include:

<details open><summary><p lang="en">Click/tap here to expand/collapse this table</p></summary>

| Linux Distribution | Chrome pre-installed | Chromium pre-installed |
|----|----|----|
| ChromeOS | :heavy_check_mark: | :x: |
| ChromiumOS | :x: | :heavy_check_mark: |
| Ubuntu (since ~12.04) | :heavy_check_mark: | :heavy_check_mark: |
| Other | :question: | :question: |

</details>

This is an obvious problem for DeGoogling. If you are on ChromeOS or ChromiumOS, it is recommended to get a different operating system. If you aren't on ChromeOS/ChromiumOS, continue reading.

* [Removing Google Chrome from Ubuntu](#Removing-Chrome-from-Ubuntu)
* [Other instructions (unavailable)](#Removing-Chrome-from-other-Linux-distributions)

## Removing Chrome from Ubuntu

<details open><summary><p lang="en">Click/tap here to expand/collapse the section on Google Chrome uninstallation on Ubuntu instructions</p></summary>

Since around 2012 (I am not sure on the origin of Chrome in Ubuntu, more research is needed. I for sure know it comes with 20.04) Google Chrome and Google Chromium come pre-installed with Ubuntu. It is a little difficult to remove (as in, more difficult than it should be) you first must uninstall Chromium, before you can uninstall Chrome. To do this, go through `Settings` > `Applications` > `Google Chromium` > `Remove`

After this, you have to uninstall Chrome. On Ubuntu 12.04 and newer, open up your preferred terminal (such as GNOME Terminal, Konsole, etc.) then run the following command (you will need super user privileges for this)

```shell
sudo apt-get remove google-chrome-stable
```

Unfortunately, uninstalling isn't enough, as the browser stays on the system, despite being uninstalled. The next step is to purge all Chrome program files from the system. To do so, run the following commands:

```shell
sudo apt purge google-chrome-stable
```

Unfortunately, we still aren't done. The next step is a bit dangerous, so follow the instructions exactly. We are going to be removing Google Chrome user data. Run the following command:

```shell
cd ~/.config
````

Ensure you stay in the `/.config` directory, the system should already tell you where you are (the indicator is in blue text) If you are unsure where you are, type either one of the following three commands:

* `l`
* `ls`
* `dir`

Now that you are in the `/.config` directory, type the following command:

```shell
rm -rf google-chrome
```

Google Chrome and Google Chromium have now been completely removed from your Linux system.

</details>

## Removing Chrome from other Linux distributions

Info on removing Google Chrome and Google Chromium from other Linux dustributions is currently unavailable.

***

## File info

<details open><summary><p lang="en">Click/tap here to expand/collapse the file info section</p></summary>

**File type:** `Markdown document (*.md *.mkd *.mdown *.markdown)`

**File version:** `1 (Tuesday, 2022, April 5th at 4:22 pm)`

**Line count (including blank lines and compiler line):** `143`

**Encoding:** `UTF-8` `With Emoji 5.0`

**All times are UTC-7 (PDT/Pacific Time)** `(Please also account for DST (Daylight Savings Time) until it is abolished/no longer followed)`

_Note that on 2022, Sunday, March 13th at 2:00 am PST, the time jumped ahead 1 hour to 3:00 am._

**You may need special rendering support for the `<details>` HTML tag being used in this document**

</details>

***

## File history

<details><summary><p lang="en">Click/tap here to expand/collapse the file history section</p></summary>

**Version 1 (2022, Tuesday, April 5th at 4:22 pm)**

**This version was made by:** [`@seanpm2001`](https://github.com/seanpm2001/)

**Changes:**

> * Started the file

> * Added a table on Linux distributions that come with Chrome/Chromium

> * Added the title section

> * Added a detailed section on removing Google Chrome and Google Chromium on Ubuntu

> * Added a placeholder section for removing Google Chrome from other Linux distributions

> * Added the file info section

> * Added the file history section

> * Added the footer section

> * No other changes in version 1

* No other other changes in version 2

**Version 2 (Coming soon)**

**Changes:**

> * Coming soon

> * No other other changes in version 2

</details>

***

### Footer

You have reached the end of this document.

( [Back to top](#Removing-Chrome-from-Linux) | [Back to GitHub](https://github.com/) | [Exit to Bing](https://www.bing.com/) | [Exit to DuckDuckGo](https://duckduckgo.com/) | [Exit to Safe.DuckDuckGo](https://safe.duckduckgo.com/) | [Exit to Ecosia](https://www.ecosia.org/) | [Exit to Swisscows](https://www.swisscows.com/) )

###### EOF

***
