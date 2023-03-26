# Recommended Filters for uBlock Origin

[![GitHub issues](https://img.shields.io/github/issues/yokoffing/filterlists)](https://github.com/yokoffing/filterlists/issues)
[![GitHub closed issues](https://badgen.net/github/closed-issues/yokoffing/filterlists?color=green)](https://github.com/yokoffing/filterlists/issues?q=is%3Aissue+is%3Aclosed)
![GitHub repo size](https://img.shields.io/github/repo-size/yokoffing/filterlists)
![GitHub](https://img.shields.io/github/license/yokoffing/filterlists?color=blue)
![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-green)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/yokoffing/filterlists)
![GitHub last commit](https://img.shields.io/github/last-commit/yokoffing/filterlists)
![GitHub Maintained](https://img.shields.io/badge/maintained-yes-green)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyokoffing%2Ffilterlists&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

![ubo default2](https://user-images.githubusercontent.com/11689349/224490854-fc3b61a5-2a5f-4ccb-9c83-b96b9fbc20d7.png)

#### NOTES
 - `uBlock filters - Unbreak`: While many of these rules seem unnecessary to me, you are free to leave it enabled, especially if you are adverse to breakage. A few strings from this list are in `Privacy Essentials`.
 - `Peter Lowe's` lists: His entries and more are in `Hagezi`, `OISD`, and `1Hosts`.
 
[uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) works best on [Firefox](https://www.mozilla.org/en-US/firefox/new/):
* [Cosmetic filters](https://github.com/gorhill/uBlock/wiki/Does-uBlock-Origin-block-ads-or-just-hide-them%3F#cosmetic-filters) to hide first-party ads (e.g., [YouTube ads](https://discourse.pi-hole.net/t/how-do-i-block-ads-on-youtube/253)), [ad-placeholders](https://www.dslreports.com/forum/r33005057-How-to-block-the-spaces-taken-up-by-blocked-ads), web [annoyances]((https://old.reddit.com/r/nextdns/comments/t8qn8c/comment/hzqrrfa/?context=3)), etc.
* [Block DNS requests](https://old.reddit.com/r/firefox/comments/l7xetb/network_priority_for_firefoxs_enhanced_tracking/gle2mqn/?web2x=&context=3) from being sent in the first place ([Firefox only](https://github.com/gorhill/uBlock/wiki/Dashboard:-Settings#disable-prefetching)) <sup>[1](https://help.nextdns.io/t/x2hzbps/using-nextdns-why-is-ublock-origin-still-catching-lots-of-ads)
* uBlock Origin can [do more](https://github.com/gorhill/uBlock/wiki/About-%22Why-uBlock-Origin-works-so-much-better-than-Pi%E2%80%91hole-does%3F%22) compared to when only blocking requests at the DNS-level
  
 ***
 
 ## Why should I use these lists?
https://how-i-experience-web-today.com/

***

## Custom Filters

### All-Purpose

1) [**HaGeZi's Pro++ DNS Blocklist**](https://github.com/hagezi/dns-blocklists#multi-pro---maximum-protection-) | [add](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.plus.txt)
<br> Pro++ combines Hagezi's own lists with respected community blocklists like [OISD](https://oisd.nl/), [Steven Black's list](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts), 1Hosts ([Pro](https://github.com/badmojr/1Hosts#1hosts-pro)), [notracking](https://github.com/notracking/hosts-blocklists), [notrack](https://gitlab.com/quidsup/notrack#notrack) list, and [more](https://github.com/hagezi/dns-blocklists/blob/main/usedsources.md#proplus). Hagezi maintains a sensible allowlist and handles false positives quickly. He also communicates known issues to community blocklists maintainers.

2) [**iam-py-test's Combo List**](https://github.com/iam-py-test/uBlock-combo) | [add](https://raw.githubusercontent.com/iam-py-test/uBlock-combo/main/list.txt)
<br> A compilation of lists to block malware, scams, phishing, and some tracking in uBO. It includes lists I mention below like Dandelion Sprout's Anti-Malware List, Actually Legitimate URL Shortener Tool, The malicious website blocklist, and iam-py-test's anti-typo list.


### Privacy

1) **Privacy Essentials** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/privacy_essentials.txt) 
<br> A curated list for advanced hardening. Includes site requests like `connect.facebook.com` and more that are not covered by uBO's [default settings](https://github.com/gorhill/uBlock/wiki/uBlock-and-others:-Blocking-ads,-trackers,-malwares#observations). It also includes my [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filterlist<sup>*[^what is this?](https://twitter.com/gorhill/status/1377613392559636486)*</sup>. Compliments uBO in [medium mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode). **Note:** This list breaks third-party logins.

2) [**Privacy Extended**](https://github.com/stephenhawk8054/PrivacyExtended) | [add](https://raw.githubusercontent.com/stephenhawk8054/PrivacyExtended/main/privacy_extended.txt)
<br> This filter list is a fork of [AdGuard Tracking Protection filter](https://filters.adtidy.org/extension/ublock/filters/3.txt). It eliminates extra allowlisting caused by [different methods](https://github.com/easylist/easylist/issues/15018) between uBO and AdGuard, and resolves issues faster if the problems are [inconsistent](https://github.com/AdguardTeam/AdguardFilters/issues/139081) between uBO and AdGuard. Privacy Extended also removes redundant filters found in [EasyPrivacy](https://easylist.to/easylist/easyprivacy.txt). 

#### URL Tracking Parameters

Add the functionality of [ClearURLs](https://github.com/ClearURLs/Addon#-clearurls-) to uBO. For either list, if you find websites with tracking parameters or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).
1) **[Actually Legitimate URL Shortener Tool](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new)** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt)
<br> As of October 2022, this list also [includes](https://github.com/DandelionSprout/adfilt/discussions/163?sort=old#discussioncomment-3956776) all entries from `AdGuard's URL Tracking Protection`.

2) **[ClearURLs for uBO](https://github.com/DandelionSprout/adfilt/tree/master/ClearURLs%20for%20uBo)** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)
<br> [optional] This list may break websites, and contains possibly-problematic rules. There is not much the maintainers can do, as this list is just the ClearURLs rules converted into a filterlist.

#### Fonts

1) **Block third party fonts** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt)
<br> [optional] A successor to `Fanboy's Anti-thirdparty Fonts`, this option blocks all web fonts from third-party providers but allows the browser to download fonts from first-party domains. I prefer this method as it does not require the extra connection to a third-party domain (speed and privacy); and, since I trust the first-party site enough to connect to it, I do not take on much additional privacy or security risks when I allow my browser to download a font directly from them.<sup>[1](https://collinmbarrett.com/block-web-fonts/)</sup> **Note:** This will break the "look and feel" of many sites.

***

## Security

1) **[Dandelion Sprout's Anti-Malware List](https://github.com/DandelionSprout/adfilt/blob/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt)
<br> Blocks heavily abused top-level domains (TLDs) and even search engine results for them. Blocks domains used in malware redirection trains and in domain parking schemes, as well as sponsored Windows PUP nags on PC guide articles. Mass blocking of domains belonging to bad IPs, and has many other subcategories that give it a solid advantage over similar lists out there.

2) **Enhanced website protection** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/enhanced_site_protection.txt)
<br> A supplement to `Dandelion Sprout's Anti-Malware List`. Block more abused TLDs for extra security.

3) **[The malicious website blocklist](https://github.com/iam-py-test/my_filters_001#filters-in-this-repo)** | [add](https://raw.githubusercontent.com/iam-py-test/my_filters_001/main/antimalware.txt)
<br> This version includes author comments, [vxvault.net's list](https://github.com/iam-py-test/vxvault_filter), [iam-py-test's anti-PUP list](https://github.com/iam-py-test/my_filters_001/blob/main/antipup.txt), and [additional rules](https://github.com/iam-py-test/my_filters_001/blob/main/special_lists/anti-malware-ubo-extension.txt) for uBO.

***

### Annoyances

1) **yokoffing's Annoyance List** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/annoyance_list.txt)
<br> A curated annoyance list that captures nuisances missed by other maintainers. It also cleans up the cludder around many sites (e.g., related articles).

2) **[Browse websites without logging in](https://github.com/DandelionSprout/adfilt/blob/master/BrowseWebsitesWithoutLoggingIn.txt)** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> [optional]

3) **[Bypass Paywalls Clean filter](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters)** | [add](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters/-/raw/main/bpc-paywall-filter.txt)
 <br> [optional] [experimental] The Bypass Paywalls Clean (BPC) filter is from the same [developer](https://gitlab.com/magnolia1234) as the [add-on](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean/) implementation. You do not need this filterlist if you use the extension. Moreover, the add-on covers more sites than the filterlist. "[Disclaimer](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters#bypass-paywalls-clean-filters): the list doesn't support as many sites as the extension/add-on does ... (and even less on iOS)."
 
4) **[Anti-paywall filters](https://github.com/liamengland1/miscfilters/blob/master/antipaywall.txt)** | [add](https://raw.githubusercontent.com/liamengland1/miscfilters/master/antipaywall.txt)
 <br> [optional] This list blocks additional third-party requests and annoyances that are not covered in the `Bypass Paywalls Clean` filterlist.

5) **[uBlock-Origin-dev-filter](https://github.com/quenhus/uBlock-Origin-dev-filter#ublock-origin-dev-filter)** | [add](https://raw.githubusercontent.com/quenhus/uBlock-Origin-dev-filter/main/dist/all_search_engines/global.txt)
 <br> [optional] Filters to block and remove copycat-websites from DuckDuckGo, Google and other search engines. Used to be specific to dev websites like StackOverflow or GitHub, but it currently supports others like Wikipedia. Supports StackOverflow + GitHub + NPM + Wikipedia + SEO Spam.
 
***

## Reading

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

## Mentions

**User comments:**
[1](https://old.reddit.com/r/uBlockOrigin/comments/t5ipte/deleted_by_user/hz5edjk/?context=2)
[2](https://old.reddit.com/r/dataisbeautiful/comments/t52qxa/oc_i_updated_our_famous_password_table_for_2022/hz4bcq8/?context=2)
[3](https://www.troddit.com/r/firefox/comments/z5auzi/firefox_not_properly_usingrecognizing_gpu_poor/iy0kru3)
[4](https://old.reddit.com/r/PFSENSE/comments/zu51od/a_better_pihole_with_pfsense_setup/j1x42mx/?context=2)

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
