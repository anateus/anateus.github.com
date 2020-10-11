---
layout: post
title: "Migrated from Posterous to Octopress"
date: 2012-08-01 20:29
comments: true
categories: 
---
I've migrated the blog from Posterous to [Octopress](http://octopress.org). Posterous was alright, but syntax highlighting was a bit annoying, and gist embedding is ugly. Plus I just wanted a little bit more control. At the same time I didn't want the various security and management headaches that basically every dynamic CMS brings with it.

I used the alternative [posterous importer provided by Jekyll](https://github.com/pepijndevos/jekyll/blob/patch-1/lib/jekyll/migrators/posterous.rb)--their default one doesn't preserve the permalinks. Before running it you should fix a bug: ```s/post\.media[2]/post.media/```. Then you can run it with ```ruby posterous.rb USERNAME PASSWORD API_TOKEN```. Presto!
