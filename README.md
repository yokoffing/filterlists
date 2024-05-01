![GitHub last commit](https://img.shields.io/github/last-commit/yokoffing/filterlists)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/yokoffing/filterlists)
![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-orange)
![GitHub Maintained](https://img.shields.io/badge/maintained-yes-yellow)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyokoffing%2Ffilterlists&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

***

# Guidelines
1) Prevent overblocking by applying the law of [diminishing returns](https://pmctraining.com/site/wp-content/uploads/2018/04/Law-of-Diminishing-Returns-CHART.png) (always blocking more ≠ better blocking experience).
2) Aim for [efficiency](https://brave.com/the-mounting-cost-of-stale-ad-blocking-rules/) without sacrificing quality (use sane, quality resources).
3) Implement the [minimum](https://reddit.com/r/uBlockOrigin/wiki/index#wiki_which_filter_lists_should_i_select.3F) number of useful lists (avoid redundancy and bloat when possible).

***

# Recommended Filters for uBlock Origin

![ubo_lists_Oct_2023](https://github.com/yokoffing/filterlists/assets/11689349/62809606-61e1-48b7-a697-58eb6e397af2)

***

### Content
1) [How To Add Custom Filters](https://github.com/yokoffing/filterlists?tab=readme-ov-file#how-to-add-custom-filters)
    1) [Privacy](https://github.com/yokoffing/filterlists?tab=readme-ov-file#privacy)
    2) [Annoyances](https://github.com/yokoffing/filterlists?tab=readme-ov-file#annoyances)
    3) [Security](https://github.com/yokoffing/filterlists?tab=readme-ov-file#security)
    4) [All-Purpose](https://github.com/yokoffing/filterlists?tab=readme-ov-file#all-purpose)
2) [Setup Examples](https://github.com/yokoffing/filterlists?tab=readme-ov-file#setup-examples)
    1) [Enhanced](https://github.com/yokoffing/filterlists?tab=readme-ov-file#enhanced)
    2) [Pro](https://github.com/yokoffing/filterlists?tab=readme-ov-file#pro)
    3) [Optimized](https://github.com/yokoffing/filterlists?tab=readme-ov-file#optimized)
3) [Block Content with Fewer Rules](https://github.com/yokoffing/filterlists?tab=readme-ov-file#block-content-with-fewer-rules)
    1) [Selectively Disable Cosmetic Filters](https://github.com/yokoffing/filterlists?tab=readme-ov-file#selectively-disable-cosmetic-filters)
    2) [Optimized Lists](https://github.com/yokoffing/filterlists?tab=readme-ov-file#optimized-lists)
4) [Advanced Settings](https://github.com/yokoffing/filterlists?tab=readme-ov-file#advanced-settings)
5) [FAQ](https://github.com/yokoffing/filterlists?tab=readme-ov-file#faq)
6) [Additional Reading](https://github.com/yokoffing/filterlists?tab=readme-ov-file#reading)
7) [Mentions](https://github.com/yokoffing/filterlists?tab=readme-ov-file#mentions)

***

# How To Add Custom Filters

### uBlock Origin
[Get](https://ublockorigin.com/) uBlock Origin (uBO), if you don't have it already.

To import custom filters into uBlock Origin:

1. Click the **subscribe** link by one of the entries below.
2. In the new tab that opens, click on **Subscribe** in the top right corner.
3. Close tab, then repeat for other lists you want to add to uBO.

> [!NOTE]
> This repo is tailored to uBlock Origin specifically. I cannot guarantee filters will work in other ad blockers.

<details><summary>Other ad blockers</summary>
    
### AdGuard
To import custom filters into AdGuard:

1. Click the **subscribe** link by one of the entries below.
2. In the new tab that opens, click on **Next**.
3. Toggle the box that says **Trusted**, then click **Subscribe**.

### AdBlock Plus
To import custom filters into Adblock Plus:

1. Click the **subscribe** link by one of the entries below.
2. In the new tab that opens, select **Yes, Add This Filter List**.

### AdBlock
To import custom filters into AdBlock:
1. Click the **subscribe** link by one of the entries below.
2. In the dialog box that pops up, press **OK**.

### Other ad blockers
**Do not use the subscribe link.** Instead, do the following:

1. Click on the title of the list from the selections below.
2. In GitHub, click `Raw` on the right-hand side of the page.
3. Copy+paste the URL to your preferred ad blocker.
4. Follow your ad blocker's instructions for adding custom lists.

</details>

***

## Privacy

1) :star: [**Privacy Essentials**](https://github.com/yokoffing/filterlists/blob/main/privacy_essentials.txt) (1k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/privacy_essentials.txt&title=privacy%20essentials)
<br> A curated list for advanced hardening. Includes [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filters<sup>*[^what is this?](https://twitter.com/gorhill/status/1377613392559636486)*</sup> and blocks requests like `connect.facebook.com` and more that are [not covered](https://github.com/gorhill/uBlock/wiki/uBlock-and-others:-Blocking-ads,-trackers,-malwares#observations) by uBO's default settings or in **Annoyances** lists.

> [!WARNING]
> **Privacy Essentials** may prevent you from logging into sites using Facebook, Google, or other third-party accounts.

2) [**yokoffing's click2load filters**](https://github.com/yokoffing/filterlists/blob/main/click2load.txt) (47 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt&title=yokoffing%20click2load%20filters)
<br> (**optional** if using `Privacy Essentials`) Turns many third-party audio and video players into [click-to-load](https://twitter.com/gorhill/status/1377613404794421258) placeholders which only load once a user clicks on it. This list speeds up page load, uses less bandwidth and browser resources, and reduces privacy exposure (by contacting fewer domains during page load). The player will load by clicking on the placeholder.

3) :star: [**Hagezi Pro mini**](https://github.com/hagezi/dns-blocklists/blob/main/adblock/pro.mini.txt) (78k domains) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.mini.txt&title=Hagezi%20Pro%20mini)
<br> A smaller version of the [Hagezi Pro DNS blocklist](https://github.com/hagezi/dns-blocklists#pro) optimized for web browsers (78k vs. 159k rules). The streamlined list excludes rules not pertinent to web browsing, like those blocking [IoT tracking](https://ovic.vic.gov.au/privacy/resources-for-organisations/internet-of-things-and-privacy-issues-and-challenges/#introduction) and [device telemetry](https://stackify.com/telemetry-tutorial/). This mini version blocks domains associated with ads, tracking, analytics, and badware.

### URL Tracking Parameters

Add the functionality of [ClearURLs](https://github.com/ClearURLs/Addon#-clearurls-) to uBO. These filter lists automatically remove tracking elements from URLs to protect your privacy when browsing the Internet.

> [!TIP]
> If you find websites with tracking parameters or experience site issues, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).

1) :star: **[Actually Legitimate URL Shortener Tool](https://github.com/DandelionSprout/adfilt/blob/master/LegitimateURLShortener.txt)** (2k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt&title=URL%20Shortener%20Tool)
<br> This list also [includes](https://github.com/DandelionSprout/adfilt/discussions/163?sort=old#discussioncomment-3956776) all entries from `AdGuard's URL Tracking Protection` as of October 2022.

2) **[ClearURLs for uBO](https://github.com/DandelionSprout/adfilt/tree/master/ClearURLs%20for%20uBo)** (700 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt&title=ClearURLS%20for%20URLs)
<br> (**optional:** This list may break websites and may contain problematic rules. There is not much the maintainers can do, as this list is just the ClearURLs rules converted into a filterlist.)

### Fonts

1) [**Block third-party fonts**](https://github.com/yokoffing/filterlists/blob/main/block_third_party_fonts.txt) (70 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt&title=Block%20third-party%20fonts)
<br> (**optional:** This will break the "look and feel" of some sites.) A successor to [Fanboy's Anti-thirdparty Fonts](https://github.com/ryanbr/fanboy-adblock/blob/master/fanboy-antifonts.txt), this option blocks all web fonts from third-party providers but allows the browser to download fonts from first-party domains. I prefer this method because it avoids third-party domains (speed and privacy benefit), and I trust the first-party site to download a font from them.<sup>[1](https://collinmbarrett.com/block-web-fonts/)</sup>
 
## Annoyances

1) :star: [**yokoffing's Annoyance List**](https://github.com/yokoffing/filterlists/blob/main/annoyance_list.txt) (1k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/annoyance_list.txt&title=yokoffing%20Annoyance%20List)
<br> A curated list that captures nuisances missed by other maintainers. It also cleans up the clutter around many sites (e.g., related articles, "read more", etc.).

2) **[Browse websites without logging in](https://github.com/DandelionSprout/adfilt/blob/master/BrowseWebsitesWithoutLoggingIn.txt)** (370 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt&title=Browse%20websites%20without%20logging%20in)
<br> This list attempts to bypass forced logins on sites.

3) [**YouTube Clear View**](https://github.com/yokoffing/filterlists/blob/main/youtube_clear_view.txt) (17 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/youtube_clear_view.txt&title=YouTube%20Clear%20View)
<br> Cleans up some of the clutter on YouTube.

### Paywalls
To most effectively bypass paywalls, use the **Bypass Paywalls Clean** [extension](https://github.com/bpc-clone/bpc_updates/releases). The blocklists are limited in what they can do and are therefore **optional**.

1) **[Bypass Paywalls Clean filter](https://github.com/bpc-clone/bypass-paywalls-clean-filters/blob/main/bpc-paywall-filter.txt)** (960 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/bpc-clone/bypass-paywalls-clean-filters/main/bpc-paywall-filter.txt&title=Bypass%20Paywalls%20Clean)
<br> You do not need this filterlist if you use the extension.
 
2) **[Anti-paywall filters](https://github.com/liamengland1/miscfilters/blob/master/antipaywall.txt)** (2k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/liamengland1/miscfilters/master/antipaywall.txt&title=Anti-paywall%20filters)
 <br> This list blocks additional third-party requests and annoyances that are not covered in the `Bypass Paywalls Clean` filterlist.

## Security

High-risk sites can expose your device to threats. These lists can prevent that by warning you before navigation or limiting what you can access.

1) [**Most Abused TLDs**](https://github.com/hagezi/dns-blocklists/blob/main/adblock/spam-tlds-ublock.txt) (213 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/spam-tlds-ublock.txt&title=Most%20Abused%20TLDs)
<br> Displays a warning before navigating to a site with an abused [TLD](https://en.wikipedia.org/wiki/Top-level_domain). Allows exceptions for legitimate sites. Merged from my own [Enhanced website protection](https://raw.githubusercontent.com/yokoffing/filterlists/main/enhanced_site_protection.txt) list, Dandelion Sprout's `Anti-Malware List`, LennyFox's `Block non-Latin TLDs` [list](https://github.com/LennyFox/Blocklists/blob/master/Block_non_latin_TLDs.txt), and [Spamhaus](https://www.spamhaus.org/statistics/tlds/) statistics.

2) **[Dandelion Sprout's Anti-Malware List](https://github.com/DandelionSprout/adfilt/blob/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)** (88k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt&title=Dandelion%20Sprout%20Anti-Malware&20List)
<br> This list blocks domains with high abuse rates and their search results. It also blocks domains involved in malware redirects, domain parking, and Windows [PUP](https://en.wikipedia.org/wiki/Potentially_unwanted_program) ads. It has many other subcategories that distinguish it from similar lists.

3) **[The malicious website blocklist](https://github.com/iam-py-test/my_filters_001/blob/main/antimalware.txt)** (38k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/iam-py-test/my_filters_001/main/antimalware.txt&title=The%20malicious%20website%20blocklist)
<br> This version includes author comments, [vxvault.net's list](https://github.com/iam-py-test/vxvault_filter), the [anti-PUP list](https://github.com/iam-py-test/my_filters_001/blob/main/antipup.txt), and [additional rules](https://github.com/iam-py-test/my_filters_001/blob/main/special_lists/anti-malware-ubo-extension.txt) for uBO.

## All-Purpose

1) [**uBlock combo list**](https://github.com/iam-py-test/uBlock-combo/blob/main/list.txt) (81k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/iam-py-test/uBlock-combo/main/list.txt&title=uBlock%20combo%20list)
<br> (**optional:** You may not want all these sub-filters, or you may prefer to use the separate lists) This list filters URL tracking [parameters](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new) as well as malware, scams, and phishing. It combines the following lists: [Dandelion Sprout's Anti-Malware List](https://github.com/yokoffing/filterlists#security), [Actually Legitimate URL Shortener Tool](https://github.com/yokoffing/filterlists#url-tracking-parameters), [The malicious website blocklist](https://github.com/yokoffing/filterlists#security), and the [anti-typo list](https://github.com/iam-py-test/my_filters_001/blob/main/antitypo.txt).

***

# Setup Examples

I've provided three setup guides: **Enhanced**, **Pro**, and **Optimized**.

## Enhanced

#### Features
* Demonstrates the power of uBO
* Blocks most cookie pop-ups, site notifications, and anti-adblock notices
* Adds additional privacy protections against URL tracking and third-party domains
* Adds security protections from known badware domains
* You have a low threshold for site breakage

#### Built-in lists
In addition to the default lists, you should also enable:
1. EasyList - Cookie Notices
2. EasyList - Notifications (if you don't already have these disabled in your browser)
3. EasyList - Social Widgets (if they bother you)
4. uBlock filters - Annoyances (anti-adblock messages)

#### Custom lists
1. yokoffing's click2load filters
2. Actually Legitimate URL Shortener Tool
3. The [Security lists](https://github.com/yokoffing/filterlists?tab=readme-ov-file#security) (if you browse high-risk categories like torrents, piracy, and third-party streaming sites, or want more peace of mind, etc.)

***

## Pro

#### Features
* Get the most value from customizing uBO
* Blocks more annoyances
* Adds significant privacy protection
* Adds security protection against abused [TLDs](https://en.wikipedia.org/wiki/Top-level_domain)
* You should be comfortable troubleshooting issues and reporting site breakage, though it should be rare

#### Built-in lists
In addition to the default lists, you should also enable:
1. AdGuard Tracking Protection (which is [purposed for uBO](https://filters.adtidy.org/extension/ublock/filters/3.txt))
2. Block Outsider Instrusion into LAN (optional)
3. AdGuard – Popup Overlays (newsletter pop-ups)
4. EasyList - Annoyances (all lists)
5. uBlock filters - Annoyances

#### Custom lists
1. Privacy Essentials
2. Hagezi's Pro Mini
3. Actually Legitimate URL Shortener Tool
4. yokoffing's Annoyance List (+ any of the other [Annoyance lists](https://github.com/yokoffing/filterlists?tab=readme-ov-file#annoyances))
5. Most Abused TLDs (optional)

***

## Optimized

* Ideal for mobile or older devices, or users who really enjoy efficiency
* Thorough blocking with reduced rule count

Replace one-for-one with [Optimized Lists](https://github.com/yokoffing/filterlists#optimized-lists).

***

# Block Content with Fewer Rules

## Selectively Disable Cosmetic Filters

One way to improve performance without compromising security or privacy is to disable [cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) on specific sites. Cosmetic filtering (aka element hiding) hides visual nuisances from the page that can't be blocked with [network filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#network-filters). Turning off cosmetic filtering when the webpage doesn't need it reduces your device's [workload](https://github.com/gorhill/uBlock/wiki/Doesn't-uBlock-Origin-add-overhead-to-page-load%3F) while still blocking unwanted network requests.

What's more, disabling the filters on specific sites provides more flexibility than [disabling cosmetic filters everywhere by default](https://github.com/gorhill/uBlock/wiki/Per-site-switches#no-cosmetic-filtering:~:text=To-,disable%20cosmetic%20filtering%20everywhere%20by%20default,-%2C%20go%20to%20the) and then re-enabling them for most sites. It made sense 10+ years ago to disable cosmetic filtering by default and only enable it for sites that needed extra coverage. Not so much now.

Modern websites often have ads, cookie banners, newsletter pop-ups, or a combination of these annoyances. Effective ad blocking now requires the cosmetic filters in **Ads** and **Annoyances** lists to remove these elements. Most devices, including [mobile devices](https://github.com/gorhill/uBlock/commit/7a768e7b1a), can handle cosmetic filtering without significant performance issues.

For a webpage where uBO seems unnecessary, [turn off cosmetic filtering for the site](https://github.com/gorhill/uBlock/wiki/Per-site-switches#no-cosmetic-filtering). This action still protects you from security and privacy risks by blocking unwanted network requests but reduces the overhead on less powerful devices during page load.

## Optimized Lists

> [!IMPORTANT]
> These lists sacrifice blocking comprehensiveness for efficiency, so expect occasional gaps in coverage when compared to their regular versions. Remember this if you run into less blocking than anticipated or when troubleshooting a website.

Another way to improve performance is to use alternative filter lists with fewer rules. **These filters are intended predominately for mobile devices.** So although uBO can handle over 500k+ rules, you don't need that many to block unwanted content effectively.

[AdGuard](https://github.com/AdguardTeam) offers filters that remove [rarely used](https://adguard.com/kb/general/ad-filtering/create-own-filters/#not_optimized-hint) rules. These optimized lists load faster and use less memory while still blocking content effectively. AdGuard creates the lists using [statistics](https://adguard.com/kb/general/ad-filtering/tracking-filter-statistics) that indicate how often each rule is applied.

> [!NOTE]
> AdGuard for [iOS](https://adguard.com/en/adguard-ios/overview.html) automatically uses optimized filters, so you don't need to manually add the iOS-specific links provided below. The guide includes these links mainly for reference, as AdGuard doesn't explicitly label the built-in filters as "optimized" even though they are.

The rule counts below compare each optimized list to its original version in uBO. The numbers are a snapshot of the rule counts at the time of writing.

### Ads

1) **[Easylist (Optimized)](https://filters.adtidy.org/extension/ublock/filters/101_optimized.txt)** (45k optimized vs. 82k rules) | [iOS version](https://filters.adtidy.org/ios/filters/101_optimized.txt) (28k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/101_optimized.txt&title=Easylist%20(Optimized))
<br> EasyList is the primary filter list that removes most adverts from web pages, including unwanted frames, images, and objects. This filter is the most popular list used by many ad blockers. 

2) **[EasyList + AdGuard Base filter (Optimized)](https://filters.adtidy.org/extension/ublock/filters/2_optimized.txt)** (73k optimized  vs. 153k rules combined) | [iOS version](https://filters.adtidy.org/ios/filters/2_optimized.txt) (34k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/2_optimized.txt&title=AdGuard%20Base%20filter%20%2B%20EasyList%20(Optimized))
<br> If Easylist (Optimized) is missing too many ads, then use this list, or stick with the built-in Easylist filter. 

3) **[AdGuard Mobile Ads filter](https://filters.adtidy.org/extension/ublock/filters/11.txt)** (9k rules optimized) | [iOS version](https://filters.adtidy.org/ios/filters/11_optimized.txt) (6k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/11.txt&title=AdGuard%20Mobile%20Ads%20)
<br> (**optional:** This filter is enabled by default when using uBO on Firefox for Android. It's an option in uBO under the category of **Ads**.) 

### Privacy

1. **[AdGuard Tracking Protection (Optimized)](https://filters.adtidy.org/extension/ublock/filters/3_optimized.txt)** (both use 100k rules; optimized removes comment lines `!`) | [iOS version](https://filters.adtidy.org/ios/filters/3_optimized.txt) (44k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/3_optimized.txt&title=AdGuard%20Tracking%20Protection%20(Optimized)%20)
<br> A comprehensive list of various online counters and web analytics tools. 

3. **[EasyPrivacy (Optimized)](https://filters.adtidy.org/extension/ublock/filters/118_optimized.txt)** (14k optimized vs. 50k rules) | [iOS version](https://filters.adtidy.org/ios/filters/118_optimized.txt) (14k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/118_optimized.txt&title=EasyPrivacy%20(Optimized))
<br> EasyPrivacy is a filter list to comprehensively block tracking on web pages, including tracking scripts and information collectors. EasyPrivacy protects personal data by stopping these trackers. This filter is the second most popular list used by many ad blockers. 

### Annoyances

1) **[Fanboy Annoyances (Optimized)](https://filters.adtidy.org/extension/ublock/filters/122_optimized.txt)** (56k optimized vs. 81k rules) |  [iOS version](https://filters.adtidy.org/ios/filters/122_optimized.txt) (11k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/122_optimized.txt&title=Fanboy%20Annoyances%20(Optimized))
<br> Hides website notifications, social media widgets, cookie notices, chat widgets, and some newsletters, thereby substantially decreasing web page loading times and uncluttering them. Includes `EasyList - Cookie Notices` and `EasyList - Social Widgets`.

2) **[AdGuard Annoyances (Optimized)](https://filters.adtidy.org/extension/ublock/filters/14_optimized.txt)** (44k optimized vs. 61k rules) | [iOS version](https://filters.adtidy.org/ios/filters/14_optimized.txt) (24k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/14_optimized.txt&title=AdGuard%20Annoyances%20(Optimized))
<br> Contains the following AdGuard filters: Cookie Notices, Popups, Mobile App Banners, Other Annoyances and Widgets. (To block social media buttons, use `AdGuard Social Media filter` as well.)

4) **[AdGuard Social Media filter (Optimized)](https://filters.adtidy.org/extension/ublock/filters/4_optimized.txt)** (16k optimized vs. 21k rules) | [iOS version](https://filters.adtidy.org/ios/filters/4_optimized.txt) (7k rules)
 | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/4_optimized.txt&title=AdGuard%20Social%20Media%20filter%20(Optimized))
<br> If you do not like numerous `Like` and `Tweet` buttons on all the popular websites on the Internet, then subscribe to this filter and you will not see them anymore.
***

# Advanced Settings

Toggle on [advanced settings](https://github.com/gorhill/uBlock/wiki/Advanced-user-features).

![advanced user](https://github.com/yokoffing/filterlists/assets/11689349/80c650dc-3f4f-4291-ab5f-53db3c42b7fc)

> [!WARNING]
 > Do not change these values blindly. Read the [description](https://github.com/gorhill/uBlock/wiki/Advanced-settings) for each preference.

| **Setting**                   | **Value** | **Description**                                                                      |
|-------------------------------|-----------|--------------------------------------------------------------------------------------|
| `autoUpdateAssetFetchPeriod`    | `10`        | auto-updater waits `x` seconds before fetching the next filterlist                                   |
| `autoUpdateDelayAfterLaunch`    | `5`         | update out-of-date filter lists `x` seconds after browser startup                                    |
| `autoUpdatePeriod`              | `1`         | uBO checks for [filter lists updates](https://www.reddit.com/r/uBlockOrigin/comments/174o7b6/comment/k4fpi4o/?context=3) every `x` hours  |
| `cnameMaxTTL`                   | `720`       | cache CNAME aliases for `x` minutes                                                                  |
| `filterAuthorMode`              | `true`      | enable [Dynamic Filtering](https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide)    |
| `updateAssetBypassBrowserCache` | `true`      | bypass cache when manually fetching a filter list more often than every hour                         |

***

# FAQ

### Which browser works best with uBO?
[uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) works [best](https://github.com/gorhill/uBlock/wiki/uBlock-Origin-works-best-on-Firefox) in Mozilla Firefox. The features supported only on [Firefox](https://www.mozilla.org/en-US/firefox/new/) include preventing unwanted [DNS requests](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#disable-prefetching) and CNAME [uncloaking](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#uncloak-canonical-names).

### Should I use a content blocker if I have Pihole, NextDNS, ControlD, etc.?
uBlock Origin can [do more](https://github.com/gorhill/uBlock/wiki/About-%22Why-uBlock-Origin-works-so-much-better-than-Pi%E2%80%91hole-does%3F%22) compared to when only blocking requests at the DNS-level, like using [cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) to hide first-party ads (e.g., [YouTube ads](https://discourse.pi-hole.net/t/how-do-i-block-ads-on-youtube/253)), [ad-placeholders](https://www.dslreports.com/forum/r33005057-How-to-block-the-spaces-taken-up-by-blocked-ads), web [annoyances]((https://reddit.com/r/nextdns/comments/t8qn8c/comment/hzqrrfa/?context=3)), etc.<sup>[1](https://help.nextdns.io/t/x2hzbps/using-nextdns-why-is-ublock-origin-still-catching-lots-of-ads)</sup>

### Why should I use these lists?
Check out [How I Experience the Web Today](https://how-i-experience-web-today.com/).

### Why did you include AdGuard's Optimize lists but not AdBlock Plus' Minified lists?
The Minified lists are part of an Adblock Plus-hosted unofficial project that was hardforked from their source lists in August 2019. They are smaller than AdGuard's Optimized lists but lack quality blocking. Because EL and EP are your primary defenses with content blocking, I wouldn't use the Minified lists.

***

# Reading

#### uBO-specific
* [How to test filters](https://www.reddit.com/r/uBlockOrigin/wiki/solutions/#wiki_how_to_test_filters)
    * gorhill's [note](https://www.reddit.com/r/uBlockOrigin/comments/xwlw7p/ubo_makes_my_ad_block_test_produce_a_worse_score/) on adblock test sites
* Toggle on [advanced settings](https://github.com/gorhill/uBlock/wiki/Advanced-user-features)
* [Dynamic filtering](https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide) | [video](https://www.youtube.com/watch?v=2lisQQmWQkY)
* [Medium Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode) | [video](https://youtu.be/2lisQQmWQkY?t=804) | [warning](https://reddit.com/r/firefox/comments/y0oce5/comment/irvpvrn/?context=1)
* [Overview of uBlock's network filtering engine](https://github.com/gorhill/uBlock/wiki/Overview-of-uBlock's-network-filtering-engine) (graph)
* [Resources Library](https://github.com/gorhill/uBlock/wiki/Resources-Library#defuser-scriptlets)
    * [Empty redirect resources](https://github.com/gorhill/uBlock/wiki/Resources-Library#empty-redirect-resources) (clicktoload.html)

#### Filter Creation
* [filterAuthorMode](https://github.com/gorhill/uBlock/wiki/Advanced-settings#filterauthormode)
* [Introduction to basic filtering syntax](https://github.com/gorhill/uBlock/wiki/Introduction-to-basic-filtering-syntax)
* [Static filter syntax](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax)
    * [!#if !](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#if-condition)
    * [$redirect](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#redirect)
    * [$denyallow,domain=](https://github.com/DandelionSprout/adfilt/blob/master/Wiki/SyntaxMeaningsThatAreActuallyHumanReadable.md#blocking-1) | [2](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#denyallow) | [AdGuard](https://github.com/AdguardTeam/AdGuardHome/wiki/Hosts-Blocklists#denyallow)
* [Syntax Meanings That Are Actually Human Readable](https://github.com/DandelionSprout/adfilt/blob/master/Wiki/SyntaxMeaningsThatAreActuallyHumanReadable.md)
    * How to block [div:nth-of-type](https://stackoverflow.com/questions/44664907/how-can-i-use-a-wildcard-in-ublock-origin)

#### Security
* [What's Your Cyberscore?](https://cybersecurity.ncsu.edu/home/whats-your-cyberscore/)

***

# Mentions

**User comments:**
[1](https://reddit.com/r/uBlockOrigin/comments/t5ipte/deleted_by_user/hz5edjk/?context=2)
[2](https://reddit.com/r/dataisbeautiful/comments/t52qxa/oc_i_updated_our_famous_password_table_for_2022/hz4bcq8/?context=2)
[3](https://reddit.com/r/firefox/comments/z5auzi/firefox_not_properly_usingrecognizing_gpu_poor/iy0kru3)
[4](https://reddit.com/r/PFSENSE/comments/zu51od/a_better_pihole_with_pfsense_setup/j1x42mx/?context=2)
[5](https://reddit.com/r/chrome/comments/11frszq/new_to_chrome_from_firefox_any_musthave/jalic90/?context=2)
[6](https://www.reddit.com/r/uBlockOrigin/comments/13jlu7p/comment/jokreju/?context=3)

#### Guides
* [FMHY: uBlock Filters](https://github.com/nbats/FMHYedit/blob/main/STORAGE.md#ublock-filters) → yokoffing/filterlists
* [knapah/uBlockOrigin-Filterlist](https://github.com/knapah/uBlockOrigin-Filterlist)
* [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists#recommendation-) → Recommendation

#### Contributions
* [Easylist](https://github.com/easylist/easylist/issues?q=author%3Ayokoffing)
* [AdGuard](https://github.com/AdguardTeam/AdguardFilters/issues?q=author%3Ayokoffing)
* [DandelionSprout](https://github.com/DandelionSprout/adfilt/issues?q=author%3Ayokoffing) / [Legitimate URL Shortener](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new)
* [uBlock Origin](https://github.com/uBlockOrigin/uAssets/issues?q=author%3Ayokoffing)
* [Hagezi DNS Blocklists](https://github.com/hagezi/dns-blocklists/issues?q=author%3Ayokoffing) | [Mentions](https://github.com/hagezi/dns-blocklists/issues?q=mentions%3Ayokoffing) | [Analysis](https://github.com/hagezi/dns-blocklists/discussions/1093)
* [1Hosts](https://github.com/badmojr/1Hosts/issues?q=author%3Ayokoffing)
* [Ghostery extension](https://github.com/ghostery/ghostery-extension/issues?q=author%3Ayokoffing)
* [DDG Tracker Radar (Blokada)](https://community.blokada.org/t/introducing-duckduckgo-tracker-radar-to-blokada/469)

<div align='center'><a href='https://www.websitecounterfree.com'><img src='https://www.websitecounterfree.com/c.php?d=9&id=19652&s=1' border='0' alt='Free Website Counter'></a><br / >
<div align='center'>23 July 2022</div>
