## Scriplets
Be sure to add [these](https://github.com/uBlock-user/uBO-Scriptlets) scriptlets to uBlock Origin.

## Recommended Filters for uBlock Origin

[![Screenshot-2022-01-09-115024.jpg](https://i.postimg.cc/jqN31xLy/Screenshot-2022-01-09-115024.jpg)](https://postimg.cc/z3zkb1wf)

**NOTES:**
 - Regarding `uBlock filters - Unbreak`: Many of these rules are now unnecessary; a few useful ones were added to `Privacy Essentails` (see below).
 - Regarding `Online Malicious` and `Peter Lowe's` lists: They are covered by using `OISD Domain Blocklist` (see below).
<BR>
 
**CUSTOM FILTERS:** <br> <br>
**OISD Domain Blocklist** (full list) | [add](https://oisd.nl/downloads)
<br> "The Best Blocklist" - OISD combines [hundreds of lists](https://oisd.nl/includedlists) and filters out the false positives. If you ever tried the [Energized project](https://github.com/EnergizedProtection/block) but became annoyed at all the breakage, then this list is for you. The maintainer is [very responsive](https://www.reddit.com/r/oisd_blocklist/comments/m6j6fg/oisd_domain_blocklist/?sort=new) to false positive reports. He also provides a domain-list version if you use Pihole, and it is listed on [NextDNS](https://nextdns.io/?from=xujj63g5). Phenominal project. [I've yet to find a list that he hasn't heard of](https://oisd.nl/allknownlists.php).

**Privacy Essentials** | [add](https://github.com/yokoffing/filterlists/blob/main/PrivacyEssentials.txt)
<br> Blocks tracking requests like `connect.facebook.com` and inconsequential webpage scripts that are not filtered by EasyPrivacy or OISD. Please open an issue to report any false positives caused by this list.
  
**Actually Legitimate URL Shortener Tool** | [add](https://github.com/DandelionSprout/adfilt/blob/master/LegitimateURLShortener.txt)
<br> + **ClearURLs for uBO** | [add](https://github.com/DandelionSprout/adfilt/blob/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt)
<br> If you find websites with useless/tracking parameters, or experience breakage, you can submit those [here](https://github.com/DandelionSprout/adfilt/discussions/163?sort=new).
 
**Browse websites without logging in** | [add](https://github.com/DandelionSprout/adfilt/blob/master/BrowseWebsitesWithoutLoggingIn.txt)
<br> Once you use it, you wonder how you got by without it!
  
**yokoffing's Annoyance List** | [add](https://github.com/yokoffing/filterlists/blob/main/AnnoyanceList)
<br> A curated annoyance list that captures nuisances missed by other maintainers. It also cleans up the cludder around many sites. I'll say it ahead of time: You're welcome ;)

 **Anti-paywall filters** | [add](https://github.com/llacb47/miscfilters/blob/master/antipaywall.txt)
 <br> Contains additional third-party requests that should be blocked.
 
 

## Why should I use these lists?
https://how-i-experience-web-today.com/
