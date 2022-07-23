# Recommended Filters for uBlock Origin

[![Screenshot-2022-01-09-115024.jpg](https://i.postimg.cc/jqN31xLy/Screenshot-2022-01-09-115024.jpg)](https://postimg.cc/z3zkb1wf)

**NOTES:**
 - Regarding `uBlock filters - Unbreak`: Many of these rules are unnecessary for me. A few were added to `Privacy Essentails` (see below).
 - Regarding `Online Malicious` and `Peter Lowe's` lists: Their entries and more are in `OISD` and `1Hosts` (see below).
 
 ***
 
## Custom Filters

### General Purpose:
1) **OISD (Full)** | [add](https://oisd.nl/downloads)
<br> "The Best Blocklist" - [OISD](https://oisd.nl/) combines [hundreds of lists](https://oisd.nl/includedlists/full) and filters out the false positives. If you ever tried the [Energized project](https://github.com/EnergizedProtection/block) but became annoyed at all the breakage, then this list is for you. The maintainer is [very responsive](https://www.reddit.com/r/oisd_blocklist/comments/s70dhx/oisd_domain_blocklist/?sort=new) to false positive reports. He also provides a domain-list version if you use Pihole, and it is listed on [NextDNS](https://nextdns.io/?from=xujj63g5). It passes the "[girlfriend test](https://www.urbandictionary.com/define.php?term=girlfriend%20test#:~:text=When%20a%20piece%20of%20technology%20is%20easy%20enough%20for%20your%20girlfriend%20to%20use%20without%20calling%20you)". Phenominal project. [I've yet to find a list that he hasn't heard of](https://oisd.nl/knownlists.php).

2) **1Hosts (Pro)** | [add](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt)
<br> [1Hosts](https://github.com/badmojr/1Hosts#safeguard-your-devices-against-pesky-ads-trackers-and-malware) is stricter than OISD; it includes domains that OISD leaves out. I've not experienced any issues using this list, though it may cause some "[minimal breakages](https://github.com/badmojr/1Hosts#quickstart-guide)" (see [feedback](https://reddit.com/r/nextdns/comments/uxwabr/kind_of_amazed_at_1hosts_pro/)). I use 1Hosts [(Lite)](https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/domains.txt) with [NextDNS](https://nextdns.io/?from=xujj63g5) while using the 1Hosts [(Pro)](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt) in [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin) because it's easier to troubleshoot any breakages, should they occur (i.e., lighter blocking at the DNS-level and stricter blocking at the browser-level).

3) **Privacy Essentials** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/PrivacyEssentials.txt)
<br> [Experimental] My curated list blocks tracking requests like `connect.facebook.com` and requests not covered by [EasyPrivacy](https://github.com/easylist/easylist#easyprivacy). It also includes my [click2load](https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt) filter list ([read more](https://twitter.com/gorhill/status/1377613392559636486)). **Please open an issue to report breakages.**

***

### Remove tracking parameters from URLs:
For either list, if you find websites with tracking parameters or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).
1) **Actually Legitimate URL Shortener Tool** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt)

2) **ClearURLs for uBO** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)

***

### Annoyances:
1) **Browse websites without logging in** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> Once you use it, you wonder how you got by without it!
  
2) **yokoffing's Annoyance List** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/AnnoyanceList)
<br> A curated annoyance list that captures nuisances missed by other maintainers. It also cleans up the cludder around many sites (e.g., related articles).

3) **Bypass Paywalls Clean filter** | [add](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters/-/raw/main/bpc-paywall-filter.txt)
 <br> [Experimental] The Bypass Paywalls Clean (BPC) filter is from the same [developer](https://gitlab.com/magnolia1234) as the [add-on](https://addons.mozilla.org/en-US/firefox/addon/bypass-paywalls-clean/) implementation. You do not need this filterlist if you use the extension. Moreover, the add-on covers more sites than the filterlist. "[Disclaimer](https://gitlab.com/magnolia1234/bypass-paywalls-clean-filters#bypass-paywalls-clean-filters): the list doesn't support as many sites as the extension/add-on does ... (and even less on iOS)."

4) **Anti-paywall filters** | [add](https://raw.githubusercontent.com/llacb47/miscfilters/master/antipaywall.txt)
 <br> This list contains additional third-party requests and annoyances that are not covered in the BPC filterlist.
 
 ***
 
## Scriplets
Add [these](https://github.com/uBlock-user/uBO-Scriptlets) scriptlets to [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin).

***

## Why should I use these lists?
https://how-i-experience-web-today.com/

***

<div align='center'><a href='https://www.websitecounterfree.com'><img src='https://www.websitecounterfree.com/c.php?d=9&id=19652&s=1' border='0' alt='Free Website Counter'></a><br / >
<div align='center'>23 July 2022</div>
