---
permalink: /mbtasux-mining-the-zeitgeist/index.html
layout: post
title: MBTAsux - Mining the zeitgeist
published: true
categories: []
---
My latest personal project is <a href="http://www.mbtasux.com">MBTAsux</a>.

For those who don't know, the <a href="http://mbta.com">MBTA</a> is Boston's public transportation authority, running subways, busses, commuter rail, and the like.

To say the least, many people are unhappy with the way it is operated. So, as a subject near and dear to my heart, I decide to make MBTAsux.

What it is: grabbing twitter messages and posting them in a format that allows easy skimming, in addition to extracting some data from the text.

The things I'm interested in:
<ul>
<li>Rudimentary sentiment analysis, i.e. how are people feeling about the MBTA right now?</li>
<li>Location tracking. I want to figure out where people complain the most. Control that for the "size" of the stations (Park and South Station would probably win the popular vote here).</li>
</ul>

Things I've yet to implement that I think are essential:
<ul>
<li>Submission form, and a mobile version of it. You know, for people who don't use twitter.</li>
<li>Map. Alas, people are not really mentioning their exact stops when they complain. So there is a really small percentage of twitters coming in that would be mappable. This brings me to the next feature:</li>
<li>A nano-format for complaining about the MBTA on twitter and other media. Something like: <i>s:kendall someone just played the Marseillaise on the hanging pipes #mbtasux</i>
</li>

How I wrote it:
<ul>
<li>Python</li>
<li>Google App Engine</li>
<li>Latest version of the code will be released soon under a BSD license.</li>
</ul>

Enjoy!</ul>
