---
layout: post
status: publish
published: true
title: Drizzle source tarball 2011.06.20 has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 1132
wordpress_url: http://blog.drizzle.org/?p=1132
date: 2011-06-21 11:15:10.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 191
  author: Drizzle 2011.06.20 released | TurboLinux Blog
  author_email: ''
  author_url: http://turbolinux.org/2011/06/drizzle-2011-06-20-released/
  date: '2011-06-22 03:37:29 +0000'
  date_gmt: '2011-06-22 11:37:29 +0000'
  content: '[...] Drizzle source tarball 2011.06.20 has been released. This is a Fremont
    development release.  Our stable GA release can be found here. [...] '
---
Drizzle source tarball, version 2011.06.20 has been released.

This is a <a href="https://launchpad.net/drizzle/fremont">Fremont</a> development release.  Our stable <a href="../../2011/06/2011/04/2011/03/15/drizzle-2011-03-12-ga-tarball-has-been-released/">GA release</a> can be found <a href="https://launchpad.net/drizzle/+milestone/2011-03-14">here</a>.

In this release:
<ul>
	<li> NOTE:  Removed the <a href="http://docs.drizzle.org/clients/drizzleadmin.html">drizzleadmin</a> utility has been removed.  The same functionality can be achieved via cleaner, alternate methods (UDS and the console plugin + ssh)</li>
	<li> DATA_DICTIONARY tables' identifiers now use MAXIMUM_IDENTIFIER_LENGTH to match INFORMATION_SCHEMA behavior</li>
	<li> Continued code refactoring - thanks to Olaf van der Spek for his contributions here</li>
	<li> Various bug fixes</li>
	<li> The <a href="http://docs.drizzle.org/testing/dbqp.html">dbqp</a> test runner now has sql-bench and crashme modes.  Docs are <a href="http://docs.drizzle.org/testing/sql-bench.html">here</a>.  You can read more <a href="http://www.wc220.com/?p=268">here</a>.</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/fremont/2011-06-20">here</a>.
