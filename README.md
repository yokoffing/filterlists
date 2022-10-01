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

![ublock lists 1](https://user-images.githubusercontent.com/11689349/193416193-9909ff8a-5e2c-4213-b151-e8d5f687d63f.png)
![ublock lists 3](https://user-images.githubusercontent.com/11689349/193416253-b89a2e66-b335-4dbb-a243-82e571beaf64.png)


**NOTES:**
 - Regarding `uBlock filters - Unbreak`: Many of these rules seem unnecessary. A few strings were added to `Privacy Essentails`.
 - Regarding `Online Malicious` and `Peter Lowe's` lists: Their entries and more are in `OISD` and `1Hosts`.
 
 ***
 
## Reading

* Toggle on [advanced settings](https://github.com/gorhill/uBlock/wiki/Advanced-user-features)
* [Dynamic filtering](https://github.com/gorhill/uBlock/wiki/Dynamic-filtering:-quick-guide)
* [Medium Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode)
* (optional) [filterAuthorMode](https://github.com/gorhill/uBlock/wiki/Advanced-settings#filterauthormode)

 ***

## Custom Filters

### General Purpose:
1) **OISD (full)** | [add](https://oisd.nl/downloads)
<br> "The Best Blocklist" - [OISD](https://oisd.nl/) combines [hundreds of lists](https://oisd.nl/includedlists/full) and filters out the false positives. If you ever tried the [Energized project](https://github.com/EnergizedProtection/block) but became annoyed at all the breakage, then this list is for you. The maintainer is [very responsive](https://www.reddit.com/r/oisd_blocklist/comments/s70dhx/oisd_domain_blocklist/?sort=new) to false positive reports. He also provides a domain-list version if you use Pihole, and it is listed on [NextDNS](https://nextdns.io/?from=xujj63g5). It passes the "[girlfriend test](https://www.urbandictionary.com/define.php?term=girlfriend%20test#:~:text=When%20a%20piece%20of%20technology%20is%20easy%20enough%20for%20your%20girlfriend%20to%20use%20without%20calling%20you)". Phenominal project. [I've yet to find a list that he hasn't heard of](https://oisd.nl/knownlists.php). Be sure to use the `full` list, not `basic`.

2) **1Hosts (Pro)** | [add](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt)
<br> [1Hosts](https://github.com/badmojr/1Hosts#safeguard-your-devices-against-pesky-ads-trackers-and-malware) [(Pro)](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt) is much stricter than OISD; it includes domains that OISD leaves out. <strike>I've not experienced any issues using this list, though it may cause some "[minimal breakages](https://github.com/badmojr/1Hosts#quickstart-guide)"</strike> (see [feedback](https://reddit.com/r/nextdns/comments/uxwabr/kind_of_amazed_at_1hosts_pro/)). I recommend using 1Hosts [(Lite)](https://github.com/badmojr/1Hosts#1hosts-lite) on [NextDNS](https://nextdns.io/?from=xujj63g5)/Pi-hole while using 1Hosts [(Pro)](https://github.com/badmojr/1Hosts#1hosts-pro) in [uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) because it's easier to troubleshoot breakages when they occur (i.e., lighter blocking at the DNS-level and stricter blocking at the browser-level).

3) **Privacy Essentials** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/PrivacyEssentials.txt) 
<br> [beta] Designed to be used with uBlock Origin in [Medium Mode](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode). My curated list blocks tracking requests like `connect.facebook.com` and requests not covered by [EasyPrivacy](https://github.com/easylist/easylist#easyprivacy). It also includes my [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filter list ([read more](https://twitter.com/gorhill/status/1377613392559636486)). **Please open an issue to report breakages.**

4) **Enhanced website protection** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/enhanced_protection.txt)
<br> [beta] **Please open an issue to report breakages.**

***

### Remove tracking parameters from URLs:
Add the functionality of [ClearURLs](https://github.com/ClearURLs/Addon) to uBO.
1) **Actually Legitimate URL Shortener Tool** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt)

2) **ClearURLs for uBO** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)

For either list, if you find websites with tracking parameters or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).

***

### Annoyances:
1) **Browse websites without logging in** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> Once you use it, you wonder how you got by without it!
  
2) **yokoffing's Annoyance List** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/AnnoyanceList)
<br> A curated annoyance list that captures nuisances missed by other maintainers. It also cleans up the cludder around many sites (e.g., related articles).

3) **Anti-paywall filters** | [add](https://raw.githubusercontent.com/llacb47/miscfilters/master/antipaywall.txt)
 <br> This list blocks additional third-party requests and annoyances that are not covered in the Bypass Paywalls Clean filterlist.

4) **Bypass Paywalls Clean filter** | [add](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters/-/raw/main/bpc-paywall-filter.txt)
 <br> [Experimental] The Bypass Paywalls Clean (BPC) filter is from the same [developer](https://gitlab.com/magnolia1234) as the [add-on](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean/) implementation. You do not need this filterlist if you use the extension. Moreover, the add-on covers more sites than the filterlist. "[Disclaimer](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters#bypass-paywalls-clean-filters): the list doesn't support as many sites as the extension/add-on does ... (and even less on iOS)."
 
 ***
 
## Scriplets
[Add](https://github.com/gorhill/uBlock/wiki/Advanced-settings#userresourceslocation) these [scriptlets](https://github.com/uBlock-user/uBO-Scriptlets) to [uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/).

***

## Why should I use these lists?
https://how-i-experience-web-today.com/

***

## Mentions

* [FMHY uBlock Filters](https://github.com/nbats/FMHYedit/blob/main/STORAGE.md#ublock-filters)

<div align='center'><a href='https://www.websitecounterfree.com'><img src='https://www.websitecounterfree.com/c.php?d=9&id=19652&s=1' border='0' alt='Free Website Counter'></a><br / >
<div align='center'>23 July 2022</div>
