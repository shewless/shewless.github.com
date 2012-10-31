---
layout: post
title: "Enabling comments with Disqus"
date: 2012-10-25 09:25
comments: true
categories: WEB
---

It appears the default *comments* option for [Octopress](http://www.octopress.org) is *true* but you will notice that your Octopress blog does not actually have a comment section.

This is because you need to create and configure a **[Disqus](http://disqus.com/)** account first:

- Register your webiste here: <http://disqus.com/admin/register/>
- Retrieve your disqus *"shortname"*
- Add the shortname to _config.yml:

``` ruby enable disqus
# Disqus Comments
disqus_short_name: unleashedweborg
disqus_show_comment_count: true
```

- You can see I also set discus_show_comment_count to true (which is optional)
