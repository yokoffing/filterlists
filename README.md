![GitHub last commit](https://img.shields.io/github/last-commit/yokoffing/filterlists)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/yokoffing/filterlists)
![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-orange)
![GitHub Maintained](https://img.shields.io/badge/maintained-yes-yellow)
[![Hits]()](https://hits.seeyoufarm.com)

***

# Guidelines
1) Prevent overblocking by applying the law of [diminishing returns]() (always blocking more ≠ better blocking experience).
2) Aim for [efficiency](https://brave.com/blog/the-mounting-cost-of-stale-ad-blocking-rules/) without sacrificing quality (use sane, quality resources).
3) Implement the [minimum](https://reddit.com/r/uBlockOrigin/wiki/index#wiki_which_filter_lists_should_i_select.3F) number of useful lists (avoid redundancy and bloat when possible).

***

# Recommended filters for uBlock Origin

![uBO lists May 2024](https://github.com/yokoffing/filterlists/assets/11689349/f1925d65-963f-4bb8-aebf-d083ee5f9825)

***
# Block Twitch ads

For Twitch adblock, I use [Violentmonkey](https://violentmonkey.github.io/get-it/) with the [AdGuard Extra](https://github.com/AdguardTeam/AdGuardExtra?tab=readme-ov-file#adguard-extra) userscript. This helps uBlock Origin block server-side ads.

You can also use Tampermonkey as a Twitch adblock solution.

# Block YouTube ads

Adblock not working on YouTube?

* uBlock Origin on Firefox should be okay. If adblock is no longer working on YouTube, check the [subreddit](https://www.reddit.com/r/uBlockOrigin/).
* If using [uBlock Origin Lite](https://github.com/uBlockOrigin/uBOL-home?tab=readme-ov-file#ubo-lite), open the popup panel and set the filtering mode to **Complete** on `youtube.com` and any other ad-invasive site.
   * For more info, see our [new section](https://github.com/yokoffing/filterlists?tab=readme-ov-file#ublock-origin-lite) on uBlock Origin Lite.

***

### Content
1) [How to add custom filters](https://github.com/yokoffing/filterlists?tab=readme-ov-file#how-to-add-custom-filters)
    1) [Privacy](https://github.com/yokoffing/filterlists?tab=readme-ov-file#privacy)
    2) [Annoyances](https://github.com/yokoffing/filterlists?tab=readme-ov-file#annoyances)
    3) [Security](https://github.com/yokoffing/filterlists?tab=readme-ov-file#security)
    4) [All-Purpose](https://github.com/yokoffing/filterlists?tab=readme-ov-file#all-purpose)
2) [Examples](https://github.com/yokoffing/filterlists?tab=readme-ov-file#setup-examples)
    1) [Enhanced](https://github.com/yokoffing/filterlists?tab=readme-ov-file#enhanced)
    2) [Pro](https://github.com/yokoffing/filterlists?tab=readme-ov-file#pro)
    3) [Optimized](https://github.com/yokoffing/filterlists?tab=readme-ov-file#optimized)
3) [Mobile adblocking: block content with fewer rules](https://github.com/yokoffing/filterlists?tab=readme-ov-file#block-content-with-fewer-rules)
    1) [Disable cosmetic filters](https://github.com/yokoffing/filterlists?tab=readme-ov-file#disable-cosmetic-filters)
    2) [Optimized lists](https://github.com/yokoffing/filterlists?tab=readme-ov-file#optimized-lists)
4) [Advanced settings](https://github.com/yokoffing/filterlists?tab=readme-ov-file#advanced-settings)
5) [uBlock Origin Lite](https://github.com/yokoffing/filterlists?tab=readme-ov-file#ublock-origin-lite)
6) [FAQ](https://github.com/yokoffing/filterlists?tab=readme-ov-file#faq)
7) [Additional reading](https://github.com/yokoffing/filterlists?tab=readme-ov-file#reading)
8) [Mentions](https://github.com/yokoffing/filterlists?tab=readme-ov-file#mentions)

***

# How to add custom filters

> [!NOTE]
> This repo is tailored specifically to uBlock Origin. I cannot guarantee filters will work in other ad blockers.

### uBlock Origin
[Get uBlock Origin](https://ublockorigin.com/) (uBO), if you don't have it already.

To import custom filters into uBlock Origin:

1. Click the **subscribe** link by one of the entries below.
2. In the new tab that opens, click on **Subscribe** in the top right corner.
3. Close the tab, then repeat for other lists you want to add to uBO.
    
### AdGuard
To import custom filters into AdGuard:

1. Click the **subscribe** link by one of the entries below.
2. In the new tab that opens, click on **Next**.
3. Toggle the box that says **Trusted**, then click **Subscribe**.

### Brave Browser
**Do not use the subscribe link.** Add your own custom filter lists from different sources just copying/pasting the `RAW` URL and pressing save changes. 

1. Click on the title of the list from the selections in this repo.
2. On GitHub, select `Raw` on the right-hand side of the page.
3. Copy the URL.
4. In a separate tab, go to `brave://adblock` in the URL bar.
5. Under **Add custom filter lists**, paste the URL and select **Add**.

<details><summary>Click me to view instructions for other adblockers</summary>

### AdBlock Plus
There is a branch specifically for Adblock Plus (ABP) syntax. Check it out [here](https://github.com/Metrokoto/filterlists-abp).

To import custom filters into ABP:

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

1) :star: [**Privacy Essentials**](https://github.com/yokoffing/filterlists/blob/main/privacy_essentials.txt) (1k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/privacy_essentials.txt&title=Privacy%20Essentials)
<br> A curated list for advanced hardening. Includes [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filters<sup>*[^what is this?](https://x.com/gorhill/status/1377613392559636486)*</sup> and blocks requests like `connect.facebook.com` and more that are [not covered](https://github.com/gorhill/uBlock/wiki/uBlock-and-others:-Blocking-ads,-trackers,-malwares#observations) by uBO's default settings or in Annoyances lists.

> [!WARNING]
> **Privacy Essentials** may prevent you from logging into sites using Facebook, Google, or other third-party accounts.

2) [**yokoffing's click2load filters**](https://github.com/yokoffing/filterlists/blob/main/click2load.txt) (47 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt&title=yokoffing's%20click2load%20filters)
<br> (**optional** if using `Privacy Essentials`) Turns many third-party audio and video players into [click-to-load](https://x.com/gorhill/status/1377613404794421258) placeholders which only load once a user clicks on it. This list speeds up page load, uses less bandwidth and browser resources, and reduces privacy exposure (by contacting fewer domains during page load). The player will load by clicking on the placeholder.

3) :star: [**Hagezi Pro mini**](https://github.com/hagezi/dns-blocklists/blob/main/adblock/pro.mini.txt) (78k domains) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.mini.txt&title=Hagezi%20Pro%20mini)
<br> A smaller version of the [Hagezi Pro DNS blocklist](https://github.com/hagezi/dns-blocklists#pro) optimized for web browsers (78k vs. 159k rules). The streamlined list excludes rules not pertinent to web browsing, like those blocking [IoT tracking](https://ovic.vic.gov.au/privacy/resources-for-organisations/internet-of-things-and-privacy-issues-and-challenges/#introduction) and [device telemetry](https://stackify.com/telemetry-tutorial/). This mini version blocks domains associated with ads, tracking, analytics, and badware.

### URL Tracking Parameters

Add the functionality of [ClearURLs](https://github.com/ClearURLs/Addon#-clearurls-) to uBO. These filter lists automatically remove tracking elements from URLs to protect your privacy when browsing the Internet.

1) :star: **[Actually Legitimate URL Shortener Tool](https://github.com/DandelionSprout/adfilt/blob/master/LegitimateURLShortener.txt)** (2k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt&title=Actually%20Legitimate%20URL%20Shortener%20Tool)
<br> This list also [includes](https://github.com/DandelionSprout/adfilt/discussions/163?sort=old#discussioncomment-3956776) all entries from `AdGuard's URL Tracking Protection` as of October 2022, but you can use both lists.

2) **[ClearURLs for uBO](https://github.com/DandelionSprout/adfilt/tree/master/ClearURLs%20for%20uBo)** (700 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt&title=ClearURLS%20for%20URLs)
<br> This list is just the rules from the ClearURLs extension converted into a filterlist.

> [!TIP]
> If you find websites with tracking parameters or experience site issues, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).

### Fonts

1) [**Block third-party fonts**](https://github.com/yokoffing/filterlists/blob/main/block_third_party_fonts.txt) (70 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt&title=Block%20third-party%20fonts)
<br> This filter blocks fonts from third-party domains, which improves page load speed and protects your privacy. There are built-in exceptions to minimize site issues, such as allowing for font icons. Overall, it's more flexible than blocking all third-party fonts outright (e.g., `$font,3p`).

> [!NOTE]
> Blocking web fonts will affect the "look and feel" of some sites.
 
## Annoyances

1) :star: [**yokoffing's Annoyance List**](https://github.com/yokoffing/filterlists/blob/main/annoyance_list.txt) (1k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/annoyance_list.txt&title=yokoffing's%20Annoyance%20List)
<br> A curated list that captures nuisances missed by other maintainers. It also cleans up the clutter around many sites (e.g., related articles, "read more", etc.).

2) **[Browse websites without logging in](https://github.com/DandelionSprout/adfilt/blob/master/BrowseWebsitesWithoutLoggingIn.txt)** (370 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt&title=Browse%20websites%20without%20logging%20in)
<br> This list attempts to bypass forced logins on sites.

3) [**YouTube Clear View**](https://github.com/yokoffing/filterlists/blob/main/youtube_clear_view.txt) (17 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yokoffing/filterlists/main/youtube_clear_view.txt&title=YouTube%20Clear%20View)
<br> Cleans up some of the clutter on YouTube.

4) [**WebSanitizer**](https://github.com/DestroyerBDT/WebSanitizer) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DestroyerBDT/WebSanitizer/refs/heads/main/WebSanitizer.txt&title=WebSanitizer)
<br> Cleans websites by removing premium content ads, privacy policies, and other unnecessary elements

### Paywalls
To most effectively bypass paywalls, use the **Bypass Paywalls Clean** [extension](https://github.com/bpc-clone/bpc_updates/releases). The blocklists are limited in what they can do and are therefore **optional**.

1) **[Bypass Paywalls Clean filter](https://gitflic.ru/project/magnolia1234/bypass-paywalls-clean-filters/blob/?file=bpc-paywall-filter.txt&branch=main)** (960 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://gitflic.ru/project/magnolia1234/bypass-paywalls-clean-filters/blob/raw?file=bpc-paywall-filter.txt&title=Bypass%20Paywalls%20Clean%20filter)
<br> You do not need this filterlist if you use the extension.
 
2) **[Anti-paywall filters](https://github.com/liamengland1/miscfilters/blob/master/antipaywall.txt)** (2k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/liamengland1/miscfilters/master/antipaywall.txt&title=Anti-paywall%20filters)
 <br> This list blocks additional third-party requests and annoyances that are not covered in the `Bypass Paywalls Clean` filterlist.

## Security

High-risk sites can expose your device to threats. These lists can prevent that by warning you before navigation or limiting what you can access.

1) [**Most Abused TLDs**](https://github.com/hagezi/dns-blocklists/blob/main/adblock/spam-tlds-ublock.txt) (213 rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/spam-tlds-ublock.txt&title=Most%20Abused%20TLDs)
<br> Displays a warning before navigating to a site with an abused [TLD](https://en.wikipedia.org/wiki/Top-level_domain). Allows exceptions for legitimate sites. Merged from my own [Enhanced website protection](https://raw.githubusercontent.com/yokoffing/filterlists/main/enhanced_site_protection.txt) list, Dandelion Sprout's `Anti-Malware List`, LennyFox's `Block non-Latin TLDs` [list](https://github.com/LennyFox/Blocklists/blob/master/Block_non_latin_TLDs.txt), and [Spamhaus](https://www.spamhaus.org/reputation-statistics/cctlds/domains/) statistics.

2) **[Dandelion Sprout's Anti-Malware List](https://github.com/DandelionSprout/adfilt/blob/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)** (88k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt&title=Dandelion%20Sprout's%20Anti-Malware%20List)
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
Balanced approach for users with a low threshold for site issues:
* Blocks most URL tracking, cookie pop-ups, and anti-adblock notices
* (optional) Adds security protections from known badware domains

#### Built-in lists
*In addition to the default lists, you should also enable:*
1. AdGuard URL Tracking Protection
2. EasyList/uBO - Cookie Notices
3. EasyList - Social Widgets (if they bother you, or you don't use them)
4. uBlock filters - Annoyances

#### Custom lists
1. yokoffing's click2load filters
2. Actually Legitimate URL Shortener Tool
3. (optional) [Security lists](https://github.com/yokoffing/filterlists?tab=readme-ov-file#security) (if you browse high-risk categories like torrents, piracy, and third-party streaming sites, or want more peace of mind, etc.)

***

## Pro

#### Features
Advanced apporach for users comfortable troubleshooting issues and reporting site breakage:
* Significant privacy protection
* Block more annoyances
* (optional) Security protection against abused [TLDs](https://en.wikipedia.org/wiki/Top-level_domain)

#### Built-in lists
*In addition to the default lists and everything under the [Enhanced setup](https://github.com/yokoffing/filterlists?tab=readme-ov-file#built-in-lists), you should also enable:*
1. (optional) AdGuard Tracking Protection, [purposed for uBO](https://filters.adtidy.org/extension/ublock/filters/3.txt)
2. EasyList - Annoyances (all lists)

#### Custom lists
*In addition to the default lists and everything under the [Enhanced setup](https://github.com/yokoffing/filterlists?tab=readme-ov-file#built-in-lists), you should also enable:*
1. Privacy Essentials (on uBO, `yokoffing's click2load filters` is included)
2. Hagezi Pro Mini
3. (optional) Block third-party fonts
4. yokoffing's Annoyance List
5. Browse websites without logging in
6. (optional) YouTube Clear View
7. (optional) Most Abused TLDs 

***

## Optimized

* Ideal for mobile or older devices, or users who really enjoy efficiency
* Thorough blocking with reduced rule count

Replace one-for-one with [Optimized Lists](https://github.com/yokoffing/filterlists#optimized-lists).

***

# Block Content with Fewer Rules

## Filter Types
Modern websites often have ads, cookie banners, newsletter pop-ups, social media icons, or any combination of these annoyances. [Cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) hide visual nuisances from the page that can't be blocked with [network filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#network-filters). But there is also a third category.

Unique to [uBlock Origin](https://github.com/gorhill/uBlock/wiki/Resources-Library) and [AdGuard](https://github.com/AdguardTeam/Scriptlets/blob/master/wiki/about-scriptlets.md) are a method of filtering called scriplets. They are small scripts that allow the content blocker to perform customized actions on websites, beyond just blocking elements. Scripts are small code snippets written in JavaScript, which perform certain functions.

This is where a powerful ad blocker like uBO or AdGuard shines, as they can block pop-ups on videos when you click them and other instrusive ads, whereas basic ad blockers only support the bare minimum of network and cosmetic filtering. You'll usually find these in built-in browser ad blockers. (I'm looking you Opera, Vivaldi, and Orion.)

## Disable Cosmetic Filters
Effective ad blocking now requires cosmetic filters in Ads and Annoyances lists to remove these elements. Most devices, including [mobile devices](https://github.com/gorhill/uBlock/commit/7a768e7b1a), can handle cosmetic filtering without significant performance issues.

However, turning off cosmetic filtering when the webpage doesn't need it reduces your device's [workload](https://github.com/gorhill/uBlock/wiki/Doesn't-uBlock-Origin-add-overhead-to-page-load%3F) while still blocking unwanted network requests.

### Option 1: Turn off cosmetic filters globally
The most optimal way to improve performance without compromising security or privacy is to disable [cosmetic filtering](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) everywhere, and then enable it on sites where it's needed. This action still protects you from security and privacy risks by blocking unwanted network requests but reduces the overhead on less powerful devices during page load.

When I was testing this feature, I was amazed at how many ads and annoyances were blocked by network filters and scriplets alone. They do most of the heavy work on non-video sites. However, there are plenty of invasive sites where cosmetic filtering is needed.

#### Instructions
To [disable cosmetic filtering everywhere](https://github.com/gorhill/uBlock/wiki/Per-site-switches#no-cosmetic-filtering:~:text=To-,disable%20cosmetic%20filtering%20everywhere%20by%20default,-%2C%20go%20to%20the), go to the **Settings** pane in the dashboard. Under the **Default behavior** heading, check the option **Disable cosmetic filtering**.

From then on, cosmetic filtering will be turned off everywhere by default. To enable it for a specific site where it is really needed, click the "eye" icon in uBO's panel.

For sites where you already know that you want to block visual elements, such as traditional search, video streaming, and news sites, you can go to the **Settings** pane in the dashboard and click on the **My rules** tab. Then, under **Temporary rules**, you can enter something like this:

```
no-cosmetic-filtering: bing.com false
no-cosmetic-filtering: cnn.com false
no-cosmetic-filtering: google.com false
no-cosmetic-filtering: twitch.tv false
no-cosmetic-filtering: youtube.com false
```

Select **Save** and then **Commit**.

To enable cosmetic filtering when you're on the site, click the uBO icon in your browser toolbar and click the "eye" icon and then the "lock" icon.

It took less than a few browsing sessions to re-enable cosmetic filtering for ad-heavy sites that I visit reguarly. But I was generally impressed with how uBO's network filters and scriplets took care of a lot annoyances using my suggested [Enhanced](https://github.com/yokoffing/filterlists?tab=readme-ov-file#enhanced) setup.

### Option 2: Selectively disable cosmetic filters
Another way to go about this is to disable [cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) on only specific sites.

For a webpage where uBO seems unnecessary, turn off cosmetic filtering for the site. Disabling cosmetic filters on specific sites is more flexible than allowing cosmetic filters everywhere by default. However, it requires you to 1) assess a site and 2) remember to disable them. This method is also less of a net benefit for your device's performance.

#### Instructions
In general, you'll want to disable cosmetic filtering for small blogs, benchmarking sites, government sites, and any other unobstrusive pages. If you already have a good idea of what those are, you can go to the **Settings** pane in the dashboard and click on the **My rules** tab. Then, under **Temporary rules**, you can enter something like this:

```
no-cosmetic-filtering: basicappleguy.com true
no-cosmetic-filtering: browserbench.org true
no-cosmetic-filtering: fda.gov true
no-cosmetic-filtering: pluralistic.net true
```

Select **Save** and then **Commit**.

More often, however, you'll disable cosmetic filtering for a site by clicking the uBO icon in your browser toolbar, selecting the "eye" icon and then the "lock" icon.

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

3) **[AdGuard Mobile Ads filter](https://filters.adtidy.org/extension/ublock/filters/11.txt)** (9k rules optimized) | [iOS version](https://filters.adtidy.org/ios/filters/11_optimized.txt) (6k rules) | [subscribe](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/11.txt&title=AdGuard%20Mobile%20Ads%20filter)
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

*Updated: 26 July 2024, after uBO devs made improvements*

| **Setting**                     | **Value**           | **Description**                                                                      |
|---------------------------------|---------------------|--------------------------------------------------------------------------------------|
| `autoUpdateAssetFetchPeriod`    | `5` `(default)`     | auto-updater waits `x` seconds before fetching the next filter list                                  |
| `autoUpdateDelayAfterLaunch`    | `10`                | update out-of-date filter lists `x` seconds after browser startup                                    |
| `autoUpdatePeriod`              | `1` `(default)`     | check every `x` hours for [filter lists updates](https://www.reddit.com/r/uBlockOrigin/comments/174o7b6/comment/k4fpi4o/?context=3)  |
| `cnameMaxTTL`                   | `480`               | (optional) cache CNAME aliases for `x` minutes                                                       |
| `filterAuthorMode`              | `true`              | enable [Dynamic Filtering](https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide)    |
| `updateAssetBypassBrowserCache` | `true`              | bypass cache when manually fetching a filter list more than once an hour                             |

***

# uBlock Origin Lite

[uBlock Origin Lite](https://github.com/uBlockOrigin/uBOL-home?tab=readme-ov-file#ubo-lite) (uBOL) is a lightweight browser extension that blocks unwanted content on websites.

The extension works efficiently by letting the browser do the heavy lifting, which means uBOL doesn't slow down your browsing experience or drain your device's resources.

**After June 2024, Google Chrome users must switch to uBOL** due to changes in Chrome's extension platform. Users of other Chromium-based browsers like Microsoft Edge, Opera, and Vivaldi will likely need to make the same change soon after.

uBOL has limited blocking capabilities because it doesn't ask for broad permissions to access and change website data. However, you can grant uBOL extra permissions to improve its blocking performance.

### Default filtering mode

To change uBOL's [default filtering mode](https://github.com/uBlockOrigin/uBOL-home?tab=readme-ov-file#ubo-lite:~:text=You%20can%20set%20the%20default%20filtering%20mode%20from%20uBOL%27s%20options%20page):

1. Open uBOL's popup panel by clicking on its icon in your browser's toolbar.
2. Click on the cogwheel icon (⚙️) to access the dashboard.
3. Choose either **Optimal** or **Complete**.

For the best balance between blocking unwanted content and low resource usage, set the default mode to **Optimal**. This will ensure better overall blocking performance without significantly impacting your browsing experience.

If you don't want to fiddle with the settings ever again and aren't concerned about resource usage, then choose **Complete**.

### Specific websites

For sites with heavy ad-injection, like YouTube, you will need to open uBOL's popup panel and choose **Complete** to block unwanted content.

To change the filtering level for a specific site:

1. Navigate to the site (if you haven't already).
2. Open uBOL's [popup panel](https://github.com/uBlockOrigin/uBOL-home?tab=readme-ov-file#ubo-lite:~:text=To%20grant%20extended%20permissions%20on%20a%20given%20site%2C%20open%20the%20popup%20panel) on the site you're on.
3. Set the filtering mode to **Complete**.
4. The page will refresh and the changes will automatically take effect.

You can also lower the filtering mode for a site by moving the slider to **Basic** or **No Filtering**.

***

# FAQ

### Which browser works best with uBO?
[uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) works [best](https://github.com/gorhill/uBlock/wiki/uBlock-Origin-works-best-on-Firefox) in Mozilla Firefox. The features supported only on [Firefox](https://www.mozilla.org/en-US/firefox/new/) include preventing unwanted [DNS requests](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#disable-prefetching) and CNAME [uncloaking](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#uncloak-canonical-names).

Starting June 2024, Google Chrome's extension platform will undergo changes that require users to transition from uBlock Origin (uBO) to uBO Lite (uBOL). It's expected that other Chromium-based browsers like Microsoft Edge, Opera, and Vivaldi, will follow suit shortly after.

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
* [Medium Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode) | [video](https://www.youtube.com/watch?v=2lisQQmWQkY&t=804s) | [warning](https://reddit.com/r/firefox/comments/y0oce5/comment/irvpvrn/?context=1)
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
* [FMHY: Adblock Filters](https://github.com/fmhy/FMHYedit/blob/main/AdblockVPNGuide.md#-adblock-filters) → yokoffing/filterlists
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
