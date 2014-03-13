---
layout: post
status: publish
published: true
title: Drizzle build 1764 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 845
wordpress_url: http://blog.drizzle.org/?p=845
date: 2010-09-14 18:12:20.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 36
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/09/14/drizzle-build-1764-tarball/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-09-14 19:47:47 +0000'
  date_gmt: '2010-09-15 03:47:47 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog Drizzle build 1764 tarball has been released: Drizzle
    source tarball based on build 1764 has been rele... http://bit.ly/bbjDRi [...] '
- id: 37
  author: A Powerful Method To Improve Residual Earnings &#8211; Dan&#8217;s Internet
    Marketing Business Blog | Dan&#039;s Internet Marketing Business Blog!
  author_email: ''
  author_url: http://askdanjohnson.com/?p=2825
  date: '2010-09-15 23:25:10 +0000'
  date_gmt: '2010-09-16 07:25:10 +0000'
  content: '[...] drizzle.org [...] '
---
Drizzle source tarball based on build 1764 has been released.

In this release:
<ul>
	<li>Using boost for locks in table_share</li>
	<li>Initial work on moving to Sphinx-based documentation</li>
	<li>random_number, random_string and counter tables added to data_dictionary</li>
	<li>libdrizzle has been moved into the drizzle tree</li>
	<li>variable defaults no longer shown automatically via drizzled --help.  To view variable values, it is suggested to use SHOW VARIABLES after server startup.  Variable default values will also be available via documentation, once it is ready.</li>
	<li>All engine-specific tests are now included in their respective plugin test directories (test suites)</li>
	<li>Continued work on command line options</li>
	<li>Continued code refactoring</li>
	<li>Various bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/+milestone/2010-09-13">here</a>
