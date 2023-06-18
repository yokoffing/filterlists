[![GitHub issues](https://img.shields.io/github/issues/yokoffing/filterlists)](https://github.com/yokoffing/filterlists/issues)
[![GitHub closed issues](https://badgen.net/github/closed-issues/yokoffing/filterlists?color=green)](https://github.com/yokoffing/filterlists/issues?q=is%3Aissue+is%3Aclosed)
![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-green)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/yokoffing/filterlists)
![GitHub last commit](https://img.shields.io/github/last-commit/yokoffing/filterlists)
![GitHub Maintained](https://img.shields.io/badge/maintained-yes-green)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyokoffing%2Ffilterlists&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

***

# Guidelines
1) Prevent overblocking by applying the law of [diminishing returns](https://pmctraining.com/site/wp-content/uploads/2018/04/Law-of-Diminishing-Returns-CHART.png) (by using [sane](https://privacyguides.org/basics/threat-modeling), quality blocklists).
2) Aim for [efficiency](https://brave.com/the-mounting-cost-of-stale-ad-blocking-rules/) without sacrificing quality (avoid redundancy and bloat when possible).
3) Implement the [minimum number](https://old.reddit.com/r/uBlockOrigin/wiki/index#wiki_which_filter_lists_should_i_select.3F) of needed and useful lists.

***

# Contents
1) [Recommended Filters for uBlock Origin](https://github.com/yokoffing/filterlists#recommended-filters-for-ublock-origin)
2) [Custom Filters](https://github.com/yokoffing/filterlists#recommended-filters-for-ublock-origin)
    1) [Privacy](https://github.com/yokoffing/filterlists#privacy)
    2) [Annoyances](https://github.com/yokoffing/filterlists#annoyances)
    3) [Security](https://github.com/yokoffing/filterlists#security)
    4) [All-Purpose](https://github.com/yokoffing/filterlists#all-purpose)
3) [Block Content with Fewer Rules](https://github.com/yokoffing/filterlists#block-content-with-fewer-rules)
    1) [Optimized Lists](https://github.com/yokoffing/filterlists#optimized-lists)
    2) [Selectively Disable Cosmetic Filters](https://github.com/yokoffing/filterlists#selectively-disable-cosmetic-filters)
4) [Setup Examples](https://github.com/yokoffing/filterlists#setup-examples)
    1) Enhanced
    2) Pro
    3) Optimized
6) [FAQ](https://github.com/yokoffing/filterlists#faq)
7) [Additional Reading](https://github.com/yokoffing/filterlists#reading)
8) [Mentions](https://github.com/yokoffing/filterlists#mentions)

***

# Recommended Filters for uBlock Origin

![default lists](https://github.com/yokoffing/filterlists/assets/11689349/e18c8c8d-3554-44ff-b163-346801471b81)

***

# Custom Filters

#### How to import custom filters into uBlock Origin (uBO):
* Choose a project from the list below
* Click `add` and copy the URL (or right click `add` and select `Copy link`)
* Under `Filter Lists > Custom` in uBO, paste the linked URL to the `Import` box
* Click `Apply Changes`

![uboCustom](https://github.com/yokoffing/filterlists/assets/11689349/797ca28e-4a2d-4ec0-8743-c61f115264eb)

***

## Privacy

1) :star: [**Privacy Essentials**](https://github.com/yokoffing/filterlists/blob/main/privacy_essentials.txt) (1k rules) | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/privacy_essentials.txt) 
<br> A curated list for advanced hardening. Includes my [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filterlist<sup>*[^what is this?](https://unofficialbird.com/gorhill/status/1377613392559636486)*</sup> and blocks requests like `connect.facebook.com` and more that are not covered by uBO's [default settings](https://github.com/gorhill/uBlock/wiki/uBlock-and-others:-Blocking-ads,-trackers,-malwares#observations) or in Annoyance lists. **Note:** This list breaks third-party logins.

2) :star: [**Hagezi's Personal DNS Blocklist**](https://github.com/hagezi/dns-blocklists#personal---my-manually-maintained-denylist-) (41k domains) | [add](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/personal.txt)
<br> Hagezi's manually maintained blocklist includes ad and tracker domains seen on the top website lists (Umbrella/Tranco/Statvoo) and extracted domains from his DNS wildcard rules. This is the core of Hagezi’s five primary DNS blocklists, which are much larger and more appropriate for DNS-level blocking.

3) [**yokoffing's click2load filters**](https://github.com/yokoffing/filterlists/blob/main/click2load.txt) (47 rules) | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt)
<br> (**optional:** Included in `Privacy Essentials`) Turns many third-party audio and video players into [click-to-load](https://unofficialbird.com/gorhill/status/1377613392559636486) placeholders which only load once a user clicks on it. This list speeds up page load, uses less bandwidth and browser resources, and reduces privacy exposure (by contacting fewer domains during page load). The player will load by clicking on the placeholder.

4) [**Privacy Extended**](https://github.com/stephenhawk8054/PrivacyExtended) (17k rules) | [add](https://raw.githubusercontent.com/stephenhawk8054/PrivacyExtended/main/privacy_extended.txt)
<br> As a fork of [AdGuard Tracking Protection](https://filters.adtidy.org/extension/ublock/filters/3.txt), this list eliminates extra allowlisting caused by different [methods](https://github.com/easylist/easylist/issues/15018) between uBO and AdGuard, and resolves issues faster if the problems are [inconsistent](https://github.com/AdguardTeam/AdguardFilters/issues/139081) between the two. Privacy Extended also removes redundant filters found in [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt).

### URL Tracking Parameters

Add the functionality of [ClearURLs](https://github.com/ClearURLs/Addon#-clearurls-) to uBO. If you find websites with tracking parameters or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).

1) :star: **[Actually Legitimate URL Shortener Tool](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new)** (2k rules) | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt)
<br> This list also [includes](https://github.com/DandelionSprout/adfilt/discussions/163?sort=old#discussioncomment-3956776) all entries from `AdGuard's URL Tracking Protection` as of October 2022.

2) **[ClearURLs for uBO](https://github.com/DandelionSprout/adfilt/tree/master/ClearURLs%20for%20uBo)** (700 rules) | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)
<br> (**optional:** This list may break websites and may contain problematic rules. There is not much the maintainers can do, as this list is just the ClearURLs rules converted into a filterlist.)

### Fonts

1) [**Block third-party fonts**](https://github.com/yokoffing/filterlists/blob/main/block_third_party_fonts.txt) (70 rules) | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt)
<br> (**optional:** This will break the "look and feel" of some sites.) A successor to [Fanboy's Anti-thirdparty Fonts](https://github.com/ryanbr/fanboy-adblock/blob/master/fanboy-antifonts.txt), this option blocks all web fonts from third-party providers but allows the browser to download fonts from first-party domains. I prefer this method because it avoids third-party domains (speed and privacy benefit), and I trust the first-party site to download a font from them.<sup>[1](https://collinmbarrett.com/block-web-fonts/)</sup>
 
## Annoyances

1) :star: [**yokoffing's Annoyance List**](https://github.com/yokoffing/filterlists/blob/main/annoyance_list.txt) (1k rules) | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/annoyance_list.txt)
<br> A curated list that captures nuisances missed by other maintainers. It also cleans up the clutter around many sites (e.g., related articles, "read more", etc.).

2) **[Browse websites without logging in](https://github.com/DandelionSprout/adfilt/blob/master/BrowseWebsitesWithoutLoggingIn.txt)** (370 rules) | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> This list attempts to bypass forced logins on sites.

3) [**YouTube Clear View**](https://github.com/yokoffing/filterlists/blob/main/youtube_clear_view.txt) (17 rules) | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/youtube_clear_view.txt)
<br> Cleans up some of the clutter on YouTube.

### Paywalls
:warning: To bypass paywalls effectively, you should use the **Bypass Paywalls Clean** extenstion for [Chrome](https://gitlab.com/magnolia1234/bypass-paywalls-chrome-clean) or [Firefox](https://gitlab.com/magnolia1234/bypass-paywalls-firefox-clean). These lists are [limited](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters#bypass-paywalls-clean-filters) in what they can do and are therefore **optional**:

1) **[Bypass Paywalls Clean filter](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters)** (960 rules) | [add](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters/-/raw/main/bpc-paywall-filter.txt)
<br> The Bypass Paywalls Clean (BPC) filter is from the same [developer](https://gitlab.com/magnolia1234) as the [add-on](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean/) implementation. You do not need this filterlist if you use the extension.
 
2) **[Anti-paywall filters](https://github.com/liamengland1/miscfilters/blob/master/antipaywall.txt)** (2k rules) | [add](https://raw.githubusercontent.com/liamengland1/miscfilters/master/antipaywall.txt)
 <br> This list blocks additional third-party requests and annoyances that are not covered in the `Bypass Paywalls Clean` filterlist.

## Security

High-risk sites can expose your device to threats. These lists can prevent that by warning you before navigation or limiting what you can access.

1) :star: [**Most Abused TLDs**](https://github.com/hagezi/dns-blocklists#most-abused-tlds---protects-against-known-malicious-top-level-domains-) (206 rules) | [add](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/spam-tlds-ublock.txt)
<br> Displays a warning before navigating to a site with an abused [TLD](https://en.wikipedia.org/wiki/Top-level_domain). Allows exceptions for legitimate sites. Merged from my own [Enhanced website protection](https://raw.githubusercontent.com/yokoffing/filterlists/main/enhanced_site_protection.txt) list, Dandelion Sprout's `Anti-Malware List`, LennyFox's `Block non-Latin TLDs` [list](https://github.com/LennyFox/Blocklists/blob/master/Block_non_latin_TLDs.txt), and [Spamhaus](https://www.spamhaus.org/statistics/tlds/) statistics.

2) **[Dandelion Sprout's Anti-Malware List](https://github.com/DandelionSprout/adfilt/blob/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)** (42k rules) | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)
<br> This list blocks domains with high abuse rates and their search results. It also blocks domains involved in malware redirects, domain parking, and Windows [PUP](https://en.wikipedia.org/wiki/Potentially_unwanted_program) ads. It has many other subcategories that distinguish it from similar lists.

3) **[The malicious website blocklist](https://github.com/iam-py-test/my_filters_001#filters-in-this-repo)** (38k rules) | [add](https://raw.githubusercontent.com/iam-py-test/my_filters_001/main/antimalware.txt)
<br> This version includes author comments, [vxvault.net's list](https://github.com/iam-py-test/vxvault_filter), the [anti-PUP list](https://github.com/iam-py-test/my_filters_001/blob/main/antipup.txt), and [additional rules](https://github.com/iam-py-test/my_filters_001/blob/main/special_lists/anti-malware-ubo-extension.txt) for uBO.

## All-Purpose

1) [**uBlock combo list**](https://github.com/iam-py-test/uBlock-combo) (81k rules) | [add](https://raw.githubusercontent.com/iam-py-test/uBlock-combo/main/list.txt)
<br> (**optional:** You may not want all these sub-filters, or you may prefer to use the separate lists) This list filters URL tracking [parameters](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new) as well as malware, scams, and phishing. It combines the following lists: [Dandelion Sprout's Anti-Malware List](https://github.com/yokoffing/filterlists#security), [Actually Legitimate URL Shortener Tool](https://github.com/yokoffing/filterlists#url-tracking-parameters), [The malicious website blocklist](https://github.com/yokoffing/filterlists#security), and the [anti-typo list](https://github.com/iam-py-test/my_filters_001/blob/main/antitypo.txt).

# Block Content with Fewer Rules

## Optimized Lists

If you want to save CPU and memory resources on your device, you can use some alternative lists that have fewer filters than the built-in ones. uBO can handle more than 300k filters, but you might not need that many to block unwanted content effectively.

The lists below are designed to be lighter and faster but still maintain high standards for content blocking. The rule counts shown are when compared to their regular list in uBO.

### Ads

1) :star: **Easylist (Optimized)** (24k vs. 67k rules) | [add](https://filters.adtidy.org/extension/ublock/filters/101_optimized.txt)
<br> EasyList is the primary filter list that removes most adverts from web pages, including unwanted frames, images, and objects. It is the most popular list used by many ad blockers.

2) **EasyList + AdGuard Base filter (Optimized)** (64k vs. 137k rules combined) | [add](https://filters.adtidy.org/extension/ublock/filters/2_optimized.txt)
<br> If Easylist (Optimized) is missing too many ads, then use this list, or stick with the built-in Easylist filter.

### Annoyances

1) :star: **Fanboy Annoyances (Optimized)** (35k vs. 91k rules) | [add](https://filters.adtidy.org/extension/ublock/filters/122_optimized.txt)
<br> Hides website notifications, social media widgets, cookie notices, chat widgets, and some newsletters, thereby substantially decreasing web page loading times and uncluttering them. (Includes `EasyList - Cookie Notices` and `EasyList - Social Widgets`)

2) :star: **AdGuard Annoyances (Optimized)** (40k vs. 68k rules) | [add](https://filters.adtidy.org/extension/ublock/filters/14_optimized.txt)
<br> Blocks irritating elements on webpages including cookie notices, third-party widgets, and in-page popups. AdGuard claims that this list doesn't duplicate `Fanboy Annoyances`, so you can use them both together. (Unlike Fanboy's version, this list doesn’t include social media widgets and buttons. To block them, you can use `AdGuard Social Media filter` separately.)

3) **AdGuard Social Media filter (Optimized)** (14k vs. 20k rules) | [add](https://filters.adtidy.org/extension/ublock/filters/4_optimized.txt)
<br> (**optional:** Redundant with `Fanboy Annoyances` / `EasyList - Social Widgets`, in my opinion) If you do not like numerous `Like` and `Tweet` buttons on all the popular websites on the Internet, then subscribe to this filter and you will not see them anymore.

## Selectively Disable Cosmetic Filters

One way to improve performance without compromising security or privacy is to [disable cosmetic filtering](https://github.com/gorhill/uBlock/wiki/Per-site-switches#no-cosmetic-filtering). Cosmetic filtering (aka element hiding) stops ads and other nuisances on the page; it only affects how the website looks. Toggling it off when you don't need it will **reduce the [workload](https://github.com/gorhill/uBlock/wiki/Doesn't-uBlock-Origin-add-overhead-to-page-load%3F) on your device while still blocking unwanted network requests**.

For sites where uBO seems unnecessary (e.g., pages with no ads), [turn off](https://github.com/gorhill/uBlock/wiki/Per-site-switches#no-cosmetic-filtering) cosmetic filtering for the site. This will still protect you from security and privacy risks (network requests) but reduce overhead to page load.

***

# Setup Examples

## Enhanced
* Demonstrates the power of uBO
* Blocks most cookie pop-ups, site notifications, and anti-adblock notices
* Adds additional privacy protections against URL tracking and third-party domains
* Adds security protections from known badware domains (optional)
* You have a low threshold for site breakage

### Lists
#### Built-in:
1. EasyList - Cookie Notices
2. EasyList - Notifications (if you don't already have these disabled in your browser)
3. EasyList - Social Widgets (if they bother you)
4. uBlock filters - Annoyances (anti-adblock messages)

#### Custom lists:
1. Hagezi's Personal DNS Blocklist
2. yokoffing's click2load filters
3. Actually Legitimate URL Shortener Tool
4. Dandelion Sprout's Anti-Malware List (if you browse high-risk categories like torrents and piracy sites, want more peace of mind, etc.)
5. The malicious website blocklist (if you browse high-risk categories like torrents and piracy sites, want more peace of mind, etc.)

***

## Pro
* The most value out of customizing uBO
* Blocks more annoyances
* Adds more privacy protection
* Adds security protection against abused [TLDs](https://en.wikipedia.org/wiki/Top-level_domain)
* You should be comfortable troubleshooting issues and reporting site breakage, though it should be rare

### Lists
#### Built-in:
1. Block Outsider Instrusion into LAN
2. AdGuard – Popup Overlays (newsletter pop-ups)
3. EasyList - Annoyances
4. uBlock filters - Annoyances
#### Custom lists:
1. Privacy Essentials
2. Hagezi's Personal DNS Blocklist
3. Privacy Extended
4. Actually Legitimate URL Shortener Tool
5. yokoffing's Annoyance List (+ any of the other [annoyance lists](https://github.com/yokoffing/filterlists#annoyances))
6. Most Abused TLDs

***

## Optimized

* Ideal for mobile or older devices, or users who really enjoy efficiency
* Thorough blocking with reduced rule count

Replace one-for-one with [Optimized Lists](https://github.com/yokoffing/filterlists#optimized-lists).

***

# FAQ

### Which browser works best with uBO?
[uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) works [best](https://github.com/gorhill/uBlock/wiki/uBlock-Origin-works-best-on-Firefox) in Mozilla Firefox. The features supported only on [Firefox](https://www.mozilla.org/en-US/firefox/new/) include preventing unwanted [DNS requests](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#disable-prefetching) and CNAME [uncloaking](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#uncloak-canonical-names).

### Should I use a content blocker if I have Pihole, NextDNS, ControlD, etc.?
uBlock Origin can [do more](https://github.com/gorhill/uBlock/wiki/About-%22Why-uBlock-Origin-works-so-much-better-than-Pi%E2%80%91hole-does%3F%22) compared to when only blocking requests at the DNS-level, like using [cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) to hide first-party ads (e.g., [YouTube ads](https://discourse.pi-hole.net/t/how-do-i-block-ads-on-youtube/253)), [ad-placeholders](https://www.dslreports.com/forum/r33005057-How-to-block-the-spaces-taken-up-by-blocked-ads), web [annoyances]((https://old.reddit.com/r/nextdns/comments/t8qn8c/comment/hzqrrfa/?context=3)), etc.<sup>[1](https://help.nextdns.io/t/x2hzbps/using-nextdns-why-is-ublock-origin-still-catching-lots-of-ads)</sup>

### Why should I use these lists?
See [here](https://how-i-experience-web-today.com/).

### Why did you include AdGuard's Optimize lists but not AdBlock Plus' Minified lists?
The Minified lists are part of an Adblock Plus-hosted unofficial project that was hardforked from their source lists in August 2019. They are smaller than AdGuard's Optimized lists but lack quality blocking. Because EL and EP are your primary defenses with content blocking, I wouldn't use the Minified lists.

***

# Reading

#### uBO-specific
* [How to test filters](https://www.reddit.com/r/uBlockOrigin/wiki/solutions/#wiki_how_to_test_filters)
* Toggle on [advanced settings](https://github.com/gorhill/uBlock/wiki/Advanced-user-features)
* [Dynamic filtering](https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide) | [video](https://www.youtube.com/watch?v=2lisQQmWQkY)
* [Medium Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode) | [video](https://youtu.be/2lisQQmWQkY?t=804) | [warning](https://old.reddit.com/r/firefox/comments/y0oce5/comment/irvpvrn/?context=1)
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
[1](https://old.reddit.com/r/uBlockOrigin/comments/t5ipte/deleted_by_user/hz5edjk/?context=2)
[2](https://old.reddit.com/r/dataisbeautiful/comments/t52qxa/oc_i_updated_our_famous_password_table_for_2022/hz4bcq8/?context=2)
[3](https://old.reddit.com/r/firefox/comments/z5auzi/firefox_not_properly_usingrecognizing_gpu_poor/iy0kru3)
[4](https://old.reddit.com/r/PFSENSE/comments/zu51od/a_better_pihole_with_pfsense_setup/j1x42mx/?context=2)
[5](https://old.reddit.com/r/chrome/comments/11frszq/new_to_chrome_from_firefox_any_musthave/jalic90/?context=2)
[6](https://www.reddit.com/r/uBlockOrigin/comments/13jlu7p/comment/jokreju/?context=3)

#### Guides
* [FMHY: uBlock Filters](https://github.com/nbats/FMHYedit/blob/main/STORAGE.md#ublock-filters) → yokoffing/filterlists
* [knapah/uBlockOrigin-Filterlist](https://github.com/knapah/uBlockOrigin-Filterlist)
* [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists#recommendation-) → Recommendation

#### Contributions
* [1Hosts](https://github.com/badmojr/1Hosts/issues?q=author%3Ayokoffing)
* [Easylist](https://github.com/easylist/easylist/issues?q=author%3Ayokoffing)
* [uBlock Origin](https://github.com/uBlockOrigin/uAssets/issues?q=author%3Ayokoffing)
* [AdGuard](https://github.com/AdguardTeam/AdguardFilters/issues?q=author%3Ayokoffing)
* [DandelionSprout](https://github.com/DandelionSprout/adfilt/issues?q=author%3Ayokoffing) / [Legitimate URL Shortener](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new)
* [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists/issues?q=author%3Ayokoffing) | [mentions](https://github.com/hagezi/dns-blocklists/issues?q=mentions%3Ayokoffing)
* [Ghostery extension](https://github.com/ghostery/ghostery-extension/issues?q=author%3Ayokoffing)
* [DDG Tracker Radar (Blokada)](https://community.blokada.org/t/introducing-duckduckgo-tracker-radar-to-blokada/469)

<div align='center'><a href='https://www.websitecounterfree.com'><img src='https://www.websitecounterfree.com/c.php?d=9&id=19652&s=1' border='0' alt='Free Website Counter'></a><br / >
<div align='center'>23 July 2022</div>
