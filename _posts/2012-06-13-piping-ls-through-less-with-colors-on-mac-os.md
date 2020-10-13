---
permalink: /piping-ls-through-less-with-colors-on-mac-os/index.html
layout: post
title: Piping ls through less with colors on Mac OS X
published: true
categories: []
---
<p>The following command will do the trick:</p>

<div class="CodeRay">
  <div class="code"><pre>CLICOLOR_FORCE=1 ls -G|less -R</pre></div>
</div>


<p>Or just add this to your <code>.bash_profile</code> file to have ls always display in color and less always able to consume color codes:</p>

<div class="CodeRay">
  <div class="code"><pre>alias ls='CLICOLOR_FORCE=1 ls -G'
alias less='less -R'</pre></div>
</div>


<p>This has been tested on 10.6.8 and should be valid for subsequent versions as well. Just a tad annoying since <code>ls</code> on Mac OS X behaves a bit differently than the standard linux one (i.e. no <code>--color</code> option).</p>
