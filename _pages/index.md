---
layout: single
title: "Deep Dot Web -UNOFFICIAL- Blog Archive and Privacy Guides"
description: "The world needs user-friendly access to the educational materials previously made available at deepdotweb.com."
header:
  image: "/free_ross.jpg"
  caption: "[freeross.org](https://freeross.org/)"
classes: wide
toc: true
permalink: /
share: true
sidebar:
  nav: "pagenav"

---


<h2>Archive: Privacy Guides, and History from DeepDotWeb.</h2>


<p>I was broken-hearted when I found out that deepdotweb got seized.</p>

<p>The world should have user-friendly access to the educational materials that were previously available on deepdotweb.com.</p>

<p>I have never bought anything from the darkweb, and have no particular inclination to use or facilitate use of the markets.</p>

<p>However, its clear that governments use the drug war to suppress their populous and take massive profit on both sides.</p>

<p>I certainly don't have any problem with the use of the markets, in fact I think they are great, when successful. I simply don't have any personal use for them, and am not trying to get caught up in all of that.</p>

<img src="https://imgur.com/T7QpFTM.png"/>

<h2>Why Build This Archive?</h2>

<p>Of course you can still visit <a href="https://web.archive.org/web/20190228074725/https://www.deepdotweb.com/">DeepDotWeb at the Internet Archive</a>, which begs the question: Why did I build this archive?</p>

<p>A few reasons.</p>

<p>1. Preserve content essential to humanity.<BR/>
2. Practice building static websites.<BR/>
3. Study Bitcoin History.<BR/>
4. Show off the content of DeepDotWeb to Highlight some of it's most important contributions.</p>

<p>Though I'm grateful for the internet archive, I thought I could do something nice with <a href="https://infominer.id/web-work/github-pages-starter-pack/">Jekyll and Github Pages</a>. </p>

<ul>
  <li><a href="https://www.wired.com/story/dark-web-drug-takedowns-deepdotweb-rebound/">WiReD: FEDS DISMANTLED THE DARK-WEB DRUG TRADE—BUT IT'S ALREADY REBUILDING</a></li>
  <li><a href="https://www.zdnet.com/article/deepdotweb-dies-with-fbi-seizure/">DeepDotWeb Dark web resource dies with FBI seizure</a></li>
</ul>

<img src="https://gir.pub/deepdotweb/deepdotweb-seized.png"/>

<h2>How to</h2>

<p><a href="https://superuser.com/questions/828907/how-to-download-a-website-from-the-archive-org-wayback-machine">Download a Website from the Archive.org Wayback Machine</a></p>

<p><code>    gem install wayback_machine_downloader</code></p>

<p>and then:</p>

<p><code>    wayback_machine_downloader https://deepdotweb.com</code></p>

<h2>Snip and Clip</h2>

<p>I'm stripping away all the header material and the comments so I can spin up a simple site, without having to host everything, and really trying to get it done asap because I have other stuff I should be doing.. </p>

<ul>
  <li><a href="https://github.com/Ruined1/HTMLArticleElementStripper">https://github.com/Ruined1/HTMLArticleElementStripper</a></li>
</ul>

<p>This app goes through and strips away everything besides what's between <code>&lt;article>...&lt;/article></code>.</p>

<p>From there, I used VSCode to prepare the content.</p>

<p>First of all, I deleted all amp pages, feed pages, comment files, memes.. whatever I could strip away quickly to be able to work with the essence.</p>

<p>I used VSCode which has a really nice search and replace funtion that works with all files in the directories it has open. But it was crashing a lot, trying to edit so many files at once.... so I deleted more and more, and edited less at a time.</p>

<p>I also learned to use RegEx to put wildcards in my search query to make it even more powerful, and speed up the process.</p>

<ul>
  <a href="https://docs.microsoft.com/en-us/visualstudio/ide/using-regular-expressions-in-visual-studio">Using Regular Expressions in Visual Studio</a></li>
</ul>

<p>I also removed the market directory and forum. For space, and really it's not my interest to connect people with darknet markets. I firmly believe, however, that anyone who desires should have free access to information on how to protect your privacy online, and the history available in the blog-feed.</p>

<ul>
  <li><a href="https://unix.stackexchange.com/questions/137419/renaming-files-with-its-path-name">Rename Files with Path Name</a></li>
</ul>

<p>There was also the matter of restructuring the format of the post title\directories to match that of Jekyll.</p>

<p>Currently this site is being published with the <a href="https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/">Minimal Mistakes Theme</a></p>

<p>Mostly because it's the one I'm most familiar with at the moment. </p>

<p>However, once everything it set up, changing themes can be relatively trival.</p>

<h2>Internet Archive Asked to take down "Terrorist Content"</h2>

<ul>
  <li><a href="https://www.google.com/amp/s/www.theverge.com/platform/amp/2019/4/11/18305968/eu-internet-terrorist-content-takedown-mistakes-internet-archive-org">Archive.org hit with hundreds of false terrorist content notices from EU</a></li>
</ul>

<p>This was another reason I was concerned that I shouldn't leave it up to the Internet Archive to protect our ability to learn best practicees for privacy online.</p>

<img src="https://gir.pub/deepdotweb/free_ross.jpg"/>