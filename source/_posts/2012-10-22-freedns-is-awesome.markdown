---
layout: post
title: "FreeDNS is awesome"
date: 2012-10-22 21:08
comments: true
categories: [WEB]
---

Purchasing your own domain name is inexpensive and is a great way to setup a personal email address or website.

You can use [Free DNS](http://freedns.afraid.org/ "Free DNS") to map your DNS to an appropriate mail server or web server.

Here is an example that allows me to use "gmail" with a personal email address <shewless@unleashed-web.org> using MX records.  

	unleashed-web.org (G)	MX	10:alt1.aspmx.l.google.com
	unleashed-web.org (G)	MX	10:alt2.aspmx.l.google.com
	unleashed-web.org (G)	MX	10:aspmx.l.google.com

In order for this to work you also need to configure [Google Apps](http://support.google.com/a/bin/answer.py?hl=en&answer=57919) to enable your email service.  This service is free for personal use.

It also points [www.unleashed-web.org](unleashed-web.org) to where this website is hosted (github):

	www.unleashed-web.org (G)	CNAME	shewless.github.com

Lastly if you want your TLD (top level domain) to work you must also add an "A record" that will point to a specific github IP address:

	unleashed-web.org (G)	A	204.232.175.78

See [This Github help article](https://help.github.com/articles/setting-up-a-custom-domain-with-pages) for more information.

This website is powered by [octopress](www.octopress.org) which can be freely deployed on [github](www.github.com).  Please keep in mind that octopress defines itself as "A blogging framework for hackers" so it all depends on how much time you want to invest.  If you're looking for something simpler there are many other way to create and host websites and blogs (most of which will cost a bit of money). 

The entire cost for your own email address and website is only the cost of the domain name itself (usually approx $15/year)!
