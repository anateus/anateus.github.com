---
permalink: /an-svnwiki-in-python/index.html
layout: post
title: An svnwiki in Python
published: true
categories: []
---
On a whim, I wrote a little wiki type thing in Python that sits on top of an SVN repo. It's incredibly basic, and basically lets you browse a repo and edit files. Natively, it supports markdown as its default display mechanism, but it would be trivial to teach it the meaning of file extensions and have other view templates.

The intended use was for a personal notebook type thing, which I decided to abandon. Basically, it's a lot like <a href="http://jottit.com">Jottit</a>, except you actually have all your data, and can replicate it between locations. Yes, it also sounds like <a href="http://atonie.org/2008/02/git-wiki">git-wiki</a>,but I only found out about that after I've finished coding this version.

Although I decided not to use it, someone else my find it useful, at least the codebase. I am offering it here with absolutely no warranty, and you can use it however you like, you can attribute or not, whatever. Since this was built for private use, i.e. no public access, I was going to integrate <code>grep </code>into it, and other such utils, leveraging unix text processing for search, mass editing, etc. So one may be interested in continuing that. I did not implement a facility for adding pages easily, though that's a trivial piece of coding.

<strong>Code:</strong> <a href="http://www.mockingeye.com/wp-content/uploads/2008/06/svnwikitar.gz" title="svnwiki">svnwiki.tar.gz</a> Change the <code>base </code>variable to reflect the location of your repo.
<strong>Requirements:</strong>
<ul>
	<li>web.py</li>
	<li>pysvn (on debian this is the <code>python-svn</code> package rather than <code>python-subversion</code>)</li>
	<li>markdown</li>
</ul>
