---
layout: post
status: publish
published: true
title: Drizzle 2010.10.01 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 890
wordpress_url: http://blog.drizzle.org/?p=890
date: 2010-10-13 18:52:40.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 45
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/10/13/drizzle-2010-10-01-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-10-13 19:59:52 +0000'
  date_gmt: '2010-10-14 03:59:52 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle 2010.10.01 tarball
    has been released: Drizzle source tarball version ... http://bit.ly/cvrDiV [...] '
---
Drizzle source tarball version 2010.10.01 has been released.

In this release:
<ul>
	<li>a large number of bug fixes - many thanks to the community for trying out our first beta release</li>
	<li>NEW REQUIREMENT:  we now require flex to build</li>
	<li>we now require HailDB instead of Embedded InnoDB *OR* HailDB</li>
	<li>sql_string is now 64 bit</li>
	<li>fixed all warnings on ICC, we now consider them errors</li>
	<li>added "make lcov" - runs our test-suite + produces lcov html reports</li>
	<li>test framework now makes use of drizzle vs. mysql</li>
	<li>replaced MY_BITMAP and Bitmap&lt;&gt; with STL standard classes</li>
	<li>innobase plugin based on innodb_plugin 1.0.6</li>
	<li>continued work on documentation</li>
	<li>continued work on transaction log</li>
	<li>added support for pre/post triggers</li>
	<li>continued code cleanup</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2010-10-11">here</a>
