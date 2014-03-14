---
layout: post
status: publish
published: true
title: Drizzle 2010.12.06 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 953
wordpress_url: http://blog.drizzle.org/?p=953
date: 2010-12-21 15:50:53.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 62
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/12/21/drizzle-2010-12-06-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-12-21 16:34:56 +0000'
  date_gmt: '2010-12-22 00:34:56 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews and drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle 2010.12.06 tarball
    has been released: Drizzle source tarball, versi... http://bit.ly/guLeIc [...] '
- id: 63
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/trackback?url=http%3A%2F%2Fblog.drizzle.org%2F2010%2F12%2F21%2Fdrizzle-2010-12-06-tarball-has-been-released%2F%3Fat_xt%3D4d11d24e25dd08f2%252C0%26sms_ss%3Dtwitter&amp;utm_source=pingb
  date: '2010-12-22 02:54:49 +0000'
  date_gmt: '2010-12-22 10:54:49 +0000'
  content: '[...] This post was mentioned on Twitter by Brian Aker. Brian Aker said:
    drizzle.org http://t.co/hHcpXxq New release for #drizzle. Introduces native UUID
    type, updates to transactional engine, bug fixes. [...] '
---
Drizzle source tarball, version 2010.12.06 beta has been released.

In this release:
<ul>
	<li>The InnoDB plugin is now based on innodb 1.1.3 from mysql 5.5.7</li>
	<li>New UUID data type</li>
	<li>Embedded InnoDB now supports ON DUPLICATE KEY UPDATE functionality</li>
	<li>HailDB can now send all messages to the drizzle logging plugins vs. just stderr</li>
	<li>Documentation additions and improvements</li>
	<li>Continued work on sys_var refactoring</li>
	<li>Continued improvements to the transaction log.  Two very tricky bugs have finally been killed thanks to <a href="http://dshrewsbury.blogspot.com/">David Shrewsbury.</a></li>
	<li>Several bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2010-12-20">here</a>
