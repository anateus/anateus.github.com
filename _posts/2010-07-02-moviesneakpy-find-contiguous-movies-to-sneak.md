---
permalink: /moviesneakpy-find-contiguous-movies-to-sneak/index.html
layout: post
title: Moviesneak.py -- Find contiguous movies to sneak into!
published: true
categories: []
---
<p><br /><strong>Edit:</strong> Fix in the comments has been applied, and the whole app is now on BitBucket, so download it from there: <a href="http://bitbucket.org/anateus/moviesneak.py">http://bitbucket.org/anateus/moviesneak.py</a></p>
<p>I'm happy to announce the release of version 0.5 of moviesneak.py, script for figuring out what movies come right after each other such that you can go from one to the next on a single ticket.</p>
<p>This version follows an age-old tradition of BASIC programs by prompting you for information step by step. The date, zipcode, movie theater, and movies you actually want to watch. Then it prints out a list of movie pairs (I doubt you're going to sit through more than two).</p>
<p>Currently a tolerance of 15 minutes is hardcoded, fairly straightforward to modify. What this mean is that if one movie starts 15 minutes before another ends, it would still recommend them as a pair, what with previews and whatnot. If the opposite is true, 15 minutes is not too suspicious a time to loiter about :&gt;</p>
<p>The code is distributed under a BSD license. It requires BeautifulSoup which I've included in my distribution, so you just need Python!</p>
<p>Happy sneaking! Don't get caught :)</p>
<p> </p>
<p><span style="text-decoration: line-through;">Download here:</span></p>
<p><span style="text-decoration: line-through;"><a href="http://logarchy.org/moviesneak-0.5.zip">moviesneak-0.5.zip</a></span></p>
