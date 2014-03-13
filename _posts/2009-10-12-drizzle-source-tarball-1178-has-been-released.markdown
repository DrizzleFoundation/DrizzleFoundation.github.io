---
layout: post
status: publish
published: true
title: Drizzle source tarball 1178 has been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 360
wordpress_url: http://blog.drizzle.org/?p=360
date: 2009-10-12 10:48:01.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball based on build 1178 has been released.  While not new for this release I wanted to make sure and point out Stewart's great tool (table_raw_reader) which reads table proto information from disk and provides a very thorough analysis of the data. Check out his <a href="http://www.flamingspork.com/blog/2009/10/01/table_raw_reader-reading-the-table-proto-from-disk-and-examining-everything/" target="_blank">blog</a> for more details.  Also in  this release are

	<li>Updates for table definitions (removal of historic Unireg FRM bits). </li>
	<li>Updates for replicationr reader</li>
	<li>Bug fixes from Diego Medina</li>
	<li>Updated Gearman functions</li>
	<li>Addition of new sleep() function via plugin</li>
	<li>Fixes for building on Snow Leaopard</li>
	<li>Remove parser storage engine dependency</li>
	<li>Added "CREATE TABLE A LIKE B ENGINE=engine"  See <a href="http://krow.livejournal.com/671235.html" target="_blank">Brian's blog</a> for more details</li>
	<li>Shrunk parser structure size by half</li>
	<li>Added Memcached information schema tables (you can now see the state of your memcached cluster)</li>

The download file and change log can be found <a href="https://launchpad.net/drizzle/trunk/bell" target="_blank">here</a>.

-Lee
