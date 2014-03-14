---
layout: post
status: publish
published: true
title: Drizzle build 1717 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 817
wordpress_url: http://blog.drizzle.org/?p=817
date: 2010-08-17 15:22:50.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 31
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/08/17/drizzle-build-1717-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-08-17 18:59:07 +0000'
  date_gmt: '2010-08-18 02:59:07 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog Drizzle build 1717 tarball has been released: Drizzle
    source tarball based on build 1717 has been rele... http://bit.ly/cxD4ZA [...] '
---
<div id="_mcePaste">Drizzle source tarball based on build 1717 has been released.</div>
<br></br>
<div id="_mcePaste">NOTE:  New dependency introduced!</div>
<div id="_mcePaste">We now require libboost-thread-dev to build.</div>
<div id="_mcePaste">Our <a href="https://launchpad.net/~drizzle-developers/+archive/ppa">ppa</a> has been updated to reflect the change.</div>
<br></br>
<div id="_mcePaste">We apologize for any inconvenience, but this gives us the following benefits:</div>
<div id="_mcePaste">
<ul>
	<li><a href="http://www.boost.org/">boost</a> threads have scope safety</li>
	<li>boost threads are completely portable (no more worrying about that stuff)</li>
	<li>They will allow us to see what is happening with threads through the Performance Schema</li>
	<li>They will allow us to eventually get rid of per-session memory, which will allow us to do more with asynchronous scheduling inside the server.</li>
</ul>
</div>
<br></br>
<div id="_mcePaste">In this release:</div>
<div id="_mcePaste">
<ul>
	<li>continued work on embedded_innodb / <a href="http://www.haildb.com/">HailDB</a></li>
	<li>continued work on <a href="http://www.8bitsofbytes.com/?p=20">logging statistics</a></li>
	<li>continued work on updating the <a href="http://inaugust.com/post/81 ">options system</a></li>
	<li>continued work on the filesystem storage engine</li>
	<li>code cleanup</li>
	<li>various bug fixes</li>
</ul>
</div>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/+milestone/2010-08-16">here</a>
