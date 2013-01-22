---
layout: post
title: "Reading everything stdin in a bash script"
date: 2013-01-22 14:27
comments: true
categories:
---

In trying to get a [collectd](http://collectd.org/) instance to send me alerts, I found out that I didn't know how to just read everything that might be piped into a bash script via standard input. You can read line by line easily using the `read` command. Just looping over it seemed pretty horrendous to me until I discovered an elegant way to do it that's perhaps canonical, but doesn't seem to pop up via quick googling:

```bash
#!/bin/bash

VALUE=$(cat)

echo "$VALUE"

```

That's it! `$(cat)` is a shorthand for `$(cat /dev/stdin)`, so presumably you can use this to read from stderr by pointing it at `/dev/stderr`.

Happy piping!


