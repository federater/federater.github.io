---
layout: home
title: FedeRater Reports
pagination: 
  enabled: true
---
Many decisions on whether to join (as a user) or defederate from (as an admin) a site are assisted by knowing what other sites tend to be in that one's orbit. FedeRater polls the cloud of public posts, and maps some of those connections in a simple report. It's not intended to be the be-all, end-all of anything, but it makes the extremes very easy to spot.

_This is not a blocklist! Domains of all varieties show up here - in particular, if someone reports a domain on the fediblock hashtag, both reporter and reported domains will [get a report](/hashtag.html) (if they aren't already here). Use both to decide if the report is trustworthy, or if you need to look further yourself.

### The machine side

For the most part, there's no human intervention: the thing just tells you what it's seen. Sometimes it can't figure out what administration endorses, sometimes it can't find a public, federated timeline (not all sites have one). Other than that, it is showing you the top 5-10 sites in each category.

Note that user count is self-reported, and some sites have patched this to display an artificially-high or -low number, or simply a random one.

FedeRater doesn't look at the content of any posts, rules, etc., or the software in use (other than to record it). If your site has a lot of interaction with edgelords because you like to lecture them, I will direct you to Popehat's Rule of Goats.

### The human side

Emoji appear next to the domain names, and this is the only "opinion" entered into the equation. Check the version explanation for the exact details, but in general there are "seed" sites, manually designated as sites that exist in their own, parallel fediverse, almost universally blocked by the mainstream one. FedeRater will then flag sites with high interaction with those sites, and those are the ones it recommends suspension for.

Other emoji next to the domain names indicate the domain's occurrence on other human-curated lists: blocks for other reasons, primarily-bot sites (which you may wish to silence to keep them from dominating hashtags or timelines, even if you otherwise approve of them), etc. Check the footnotes of each report to see what parameters it was generated under, and when.

Current version: [🧁](version-cupcake.html]
