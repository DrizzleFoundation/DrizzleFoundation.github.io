---
layout: post
status: publish
published: true
title: Drizzle 2010.11.04 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 936
wordpress_url: http://blog.drizzle.org/?p=936
date: 2010-11-24 07:59:28.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 58
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/11/24/drizzle-2010-11-04-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-11-24 09:13:36 +0000'
  date_gmt: '2010-11-24 17:13:36 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews and Venkat, drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle 2010.11.04 tarball
    has been released: Drizzle source tarball, versi... http://bit.ly/i0MYNG [...] '
- id: 59
  author: sapphirecat
  author_email: no.thanks@example.com
  author_url: http://www.sapphirepaw.org/
  date: '2010-11-24 13:23:52 +0000'
  date_gmt: '2010-11-24 21:23:52 +0000'
  content: 'Broken link on the docs, it''s missing the final L: http://docs.drizzle.org/barriers.html'
- id: 60
  author: Patrick Crews
  author_email: gleebix@gmail.com
  author_url: http://wc220.com
  date: '2010-11-24 15:02:53 +0000'
  date_gmt: '2010-11-24 23:02:53 +0000'
  content: |-
    @sapphirecat:
    Thanks for pointing this out - fixed now : )
---
Drizzle source tarball, version 2010.11.04 has been released, just in time for Thanksgiving : )

This is a beta-quality release.

In this release:
<ul>
	<li>NOTE: Drizzle now recognizes mixed-case table names.  Previously, such names were converted to lower-case.  Now mixed-case is accepted and preserved, but previously created tables will still be lower-case.</li>
	<li>Updated innobase plugin to be based on innodb_plugin 1.0.9</li>
	<li>Added support for barriers.  These are objects that assist with coordinating several connections.  Please see the <a href="http://docs.drizzle.org/barriers.html">docs</a> for more details</li>
	<li>New DATA_DICTIONARY table functions for user convenience:
- USER_BARRIERS
- USER_DEFINED_VARIABLES
- USER_LOCKS
- USER_SAVEPOINTS</li>
	<li> Additional debugging functionality for transaction_reader (utility for the transaction log)</li>
	<li> EXECUTE can now be CONCURRENT and with NO RETURN</li>
	<li> Continued code refactoring</li>
	<li> Various Bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/+milestone/2010-11-22">here</a>
