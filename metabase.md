---
title: "Metabase"
---
The [metabase](metabase.csv) is a CSV derived from the database, of all the known links between admin/mods and other instances.

"Known" is doing a lot of work:

* not all mods are known
* boosts/mentions are samples only
* links expire (this file is currently shorter-term than the one used to generate FedeRater reports)

You can import this into a database and do your own rating. If you'd like a list of everyone who interacts with [FediNuke](https://seirdy.one/pb/FediNuke.txt) sites, import both into your database and run a query against it to filter for only interactions with FediNuke sites.

`select metabase.* from metabase inner join FediNuke on metabase.interact = FediNuke.field1 order by instance`

This won't give you a safe list of sites to block, just a list of sites to look more closely at.

A slightly more complicated version of this query is how the FedeRater emoji are assigned. The seed lists are much smaller than FediNuke:

* no sites that cause false positives
* lists reflect a single cluster type
* interaction types are weighted (Relay/Local Bubble >>>> Mention/Boost)

__The Metabase does not include federated timeline or non-admin user interactions, even on single-user instances.__
