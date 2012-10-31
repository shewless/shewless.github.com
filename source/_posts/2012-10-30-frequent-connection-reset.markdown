---
layout: post
title: "Frequent Connection Reset"
date: 2012-10-30 23:20
comments: true
categories: WEB
---

Uhoh.. every once and a while I get this error when trying to access my site: <http://www.unleashed-web.org>.  When I hit "refresh" the problem vanishes (for a short time).

{% img center /images/2012-10-30-frequent-connection-reset/problemLoading.png %}

My site is hosted by [Github](http://github.com).  I began searching other websites that are hosted by github and I noticed that I would occasionally get the same *"The connection was reset"* error.

I contacted the Github support team and told them about the problem.  They were very fast to investigate and respond:

> This is a known issue with some of our DDoS hardware that's in place.  We're currently working with our hosting provider to resolve this issue.  Sorry for the inconvenience.

After some googling I realized that the Github servers have recently suffered some [DDOS](https://twitter.com/github/status/259029493669310464) attacks and it seems as though they don't have a fully working solution in place to deal with that yet.

Thank you to the github team for diligently working through the issues!  In the mean time we'll need to *refresh* our browsers every once and awhile to load github hosted websites.
