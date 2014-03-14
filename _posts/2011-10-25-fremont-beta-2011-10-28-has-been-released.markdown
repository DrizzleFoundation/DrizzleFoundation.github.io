---
layout: post
status: publish
published: true
title: Fremont beta (2011.10.28) has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 1187
wordpress_url: http://blog.drizzle.org/?p=1187
date: 2011-10-25 13:43:10.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 197
  author: dbqp and Xtrabackup testing - MySQL Performance Blog
  author_email: ''
  author_url: http://www.mysqlperformanceblog.com/2011/11/16/dbqp-and-xtrabackup-testing/
  date: '2012-04-17 23:54:48 +0000'
  date_gmt: '2012-04-18 07:54:48 +0000'
  content: '[...] this testing goodness will also find its way into Drizzle (which
    currently has a 7.1 beta out).  We definitely need to see some Xtrabackup test
    cases for Drizzle’s version of the tool (mwa [...] '
---
It is finally here!

The Fremont beta is out and ready to be tested.

In this release:
<ul>
	<li><a href="http://dshrewsbury.blogspot.com/2011/03/multi-master-support-in-drizzle.html">Multi-master replication</a> (no conflict resolution)</li>
	<li>UUID's for replication (thanks to <a href="http://www.8bitsofbytes.com/">Joe Daly</a>)</li>
	<li><a href="http://www.flamingspork.com/blog/2011/05/13/drizzle-json-interface-merged/">JSON interface</a> available</li>
	<li>Percona Innodb patches merged</li>
	<li><a href="http://www.percona.com/software/percona-xtrabackup/">Xtrabackup</a> <a href="http://www.flamingspork.com/blog/2011/03/24/drizzle-online-backup-with-xtrabackup/">in-tree</a></li>
	<li>IPV6 data type available</li>
	<li><a href="http://hackdrizzle.com/drizzle-merges-query-log/">query login</a> plugin (syslog) is enabled / on by default</li>
	<li>Ability to <a href="http://developian.blogspot.com/2011/08/zeromq-support-in-drizzle.html">publish transactions to zeromq</a></li>
	<li>Improvements to logging stats plugin</li>
	<li>Work on stored procedure interface</li>
	<li>Removal of drizzleadmin utility</li>
	<li>Removal of HailDB engine</li>
	<li>Improvements to <a href="http://docs.drizzle.org/">Drizzle documentation</a> (thanks to <a href="http://hackdrizzle.com/">Daniel Nichter</a>, <a href="http://openlife.cc/blog">Henrik Ingo</a>, and <a href="http://vjsamuel.wordpress.com/">Vijay Samuel</a> for their efforts)</li>
	<li>Revamped testing system with suites of randgen, sysbench, sql-bench, and crashme tests</li>
	<li>Continued code refactoring</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/fremont/2011-10-25">here</a>
