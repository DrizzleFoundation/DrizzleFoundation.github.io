---
layout: post
status: publish
published: true
title: Drizzle build 1802 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 857
wordpress_url: http://blog.drizzle.org/?p=857
date: 2010-09-29 09:08:50.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 41
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/09/29/drizzle-build-1802-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-09-29 11:11:54 +0000'
  date_gmt: '2010-09-29 19:11:54 +0000'
  content: '[...] This post was mentioned on Twitter by Monty Taylor, drizzlenews.
    drizzlenews said: DrizzleBlog Drizzle build 1802 tarball has been released: Drizzle
    source tarball based on build 1802 has been rele... http://bit.ly/cRFBzO [...] '
---
Drizzle source tarball based on build 1802 has been released.

This is our Drizzle7 beta release.  Please test away!

In this release:
<ul>
	<li>kernel options uses boost program_options, replaced my_getopt</li>
	<li>csv, archive, and blackhole tables are not enabled by default, need --plugin-add &lt;name&gt; to use them</li>
	<li>significant work on the transaction log - testing + bug fixes.  This provides the infrastructure for replication.</li>
	<li>drizzledump can now be used to migrate MySQL-&gt;Drizzle directly (no intermediate dump files)</li>
	<li>session/memory uses boost specific</li>
	<li>thread system based on boost</li>
	<li>improvements in configuration file processing</li>
	<li>merge of latest from PBXT 1.0.11-7 + new PBXT tests and bug fixes</li>
	<li>introduction of session performance table (not built by default)</li>
	<li>initial work on catalog support</li>
	<li>introduction of Sphinx-based documentation within the source tree</li>
	<li>stress testing of the data_dictionary tables (high concurrency scenarios) via the randgen</li>
	<li>timestamps are now 64 bit and ISO compliant</li>
	<li>4 byte enum - able to handle very large enum operations</li>
	<li>dates are now 4 bytes - allows us to support a full range of values</li>
	<li>IO cleanup</li>
	<li>40 bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2010-09-27">here</a>
