---
layout: post
status: publish
published: true
title: Drizzle build 1742 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 842
wordpress_url: http://blog.drizzle.org/?p=842
date: 2010-08-31 12:03:40.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 35
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/08/31/drizzle-build-1742-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-08-31 14:42:04 +0000'
  date_gmt: '2010-08-31 22:42:04 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle build 1742 tarball
    has been released: Drizzle source tarball based on... http://bit.ly/bmoyOw [...] '
---
Drizzle source tarball based on build 1742 has been released.
<br><br>
In this release:
<ul>
	<li>*Continued work on <a href="http://www.8bitsofbytes.com/">logging statistics</a> - added a table to the scoreboard that gives memory usage and size</li>
	<li> print stack trace and stack dump have been removed.  As we use gcc for a majority of our builds, we are now using the built-in backtrace ability.  Added crash and shutdown functions for use in testing.  See <a href="https://blueprints.launchpad.net/drizzle/+spec/remove-print-stack-trace">blueprint</a> for more details</li>
	<li> FOREIGN KEY info is now put into the table proto on CREATE TABLE, no longer just passed to the engine</li>
	<li> SHOW CREATE TABLE now uses the table proto</li>
	<li> Packages available for <a href="http://packages.debian.org/unstable/main/drizzle">Debian</a> and <a href="https://launchpad.net/ubuntu/+source/drizzle">Ubuntu</a></li>
	<li> Removed static instances from plugins</li>
	<li> Continued code cleanup</li>
	<li> Various bug fixes</li>
</ul>
<br><br>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/dexter/2010-08-30">here</a>
