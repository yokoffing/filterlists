## Recommended Filters for uBlock Origin

[![Screenshot-2022-01-09-115024.jpg](https://i.postimg.cc/jqN31xLy/Screenshot-2022-01-09-115024.jpg)](https://postimg.cc/z3zkb1wf)

**NOTES:**
 - Regarding `uBlock filters - Unbreak`: Many of these rules are unnecessary for me. A few were added to `Privacy Essentails` (see below).
 - Regarding `Online Malicious` and `Peter Lowe's` lists: They are covered by using `OISD (Full)` (see below).
 
## Custom Filters

### General Purpose:
1) **OISD (Full)** | [add](https://oisd.nl/downloads)
<br> "The Best Blocklist" - OISD combines [hundreds of lists](https://oisd.nl/includedlists/full) and filters out the false positives. If you ever tried the [Energized project](https://github.com/EnergizedProtection/block) but became annoyed at all the breakage, then this list is for you. The maintainer is [very responsive](https://www.reddit.com/r/oisd_blocklist/comments/s70dhx/oisd_domain_blocklist/?sort=new) to false positive reports. He also provides a domain-list version if you use Pihole, and it is listed on [NextDNS](https://nextdns.io/?from=xujj63g5). Phenominal project. [I've yet to find a list that he hasn't heard of](https://oisd.nl/knownlists.php).

2) **1Hosts (Pro)** | [add](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt)
<br> 1Hosts (Pro) is stricter than OISD and thus it includes domains that OISD leaves out. While 1Hosts (Pro) claims to cause "[some minimal breakages](https://github.com/badmojr/1Hosts#quickstart-guide)", I've not experienced any issues myself. However, to err on the side of less potential breakage, I use 1Hosts [(Lite)](https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/domains.txt) with [NextDNS](https://nextdns.io/?from=xujj63g5) while using the 1Hosts [(Pro)](https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt) in [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin) (because it's easier to troubleshoot any breakages, should they occur).

3) **Privacy Essentials** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/PrivacyEssentials.txt)
<br> [Experimental] My curated list blocks tracking requests like `connect.facebook.com` and inconsequential webpage scripts that are not filtered by EasyPrivacy or OISD. **Please open an issue to report breakages caused by this list.**

### Remove tracking parameters from URLs:
For either list, if you find websites with tracking parameters, or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).
1) **Actually Legitimate URL Shortener Tool** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt)

2) **ClearURLs for uBO** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)

### Annoyances:
1) **Browse websites without logging in** | [add](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> Once you use it, you wonder how you got by without it!
  
2) **yokoffing's Annoyance List** | [add](https://raw.githubusercontent.com/yokoffing/filterlists/main/AnnoyanceList)
<br> A curated annoyance list that captures nuisances missed by other maintainers. It also cleans up the cludder around many sites. I'll say it ahead of time: You're welcome ;)

3) **Anti-paywall filters** | [add](https://raw.githubusercontent.com/llacb47/miscfilters/master/antipaywall.txt)
 <br> Contains additional third-party requests that should be blocked.
 
 ## Scriplets
Add [these](https://github.com/uBlock-user/uBO-Scriptlets) scriptlets to [uBlock Origin](https://github.com/gorhill/uBlock#ublock-origin).

## Why should I use these lists?
https://how-i-experience-web-today.com/
