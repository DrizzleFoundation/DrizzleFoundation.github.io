---
layout: post
status: publish
published: true
title: Drizzle 2011.02.09 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 1015
wordpress_url: http://blog.drizzle.org/?p=1015
date: 2011-02-01 15:17:19.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 70
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2011/02/01/drizzle-2011-02-09-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2011-02-01 16:24:30 +0000'
  date_gmt: '2011-02-02 00:24:30 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle 2011.02.09 tarball
    has been released: Drizzle source tarball, versi... http://bit.ly/fOF17P [...] '
---
Drizzle source tarball, version 2011.02.09 has been released.

We'd like to thank everyone that has been providing feedback and bug reports -  please keep them coming!  We are making some huge strides in the quality and availability of our <a href="http://docs.drizzle.org/">documentation</a> so please be sure to check it out and write up a <a href="http://docs.drizzle.org/clients/drizzledump.html">bug</a> if something is missing or wrong : )
We're also quite excited to have a working SQLAlchemy dialect!  We plan on incorporating more of that project's tests into our own build system soon.  Thanks to <a href="http://inaugust.com/">Monty Taylor</a> for making this happen.

In this release:
<ul>
	<li>Continued progress on catalogs.</li>
	<li><a href="http://www.haildb.com/">HailDB</a> now can get rec_per_key index statistics (via <a href="https://launchpad.net/haildb/+milestone/cairo">HailDB 2.3 cairo</a> API)</li>
	<li><a href="http://www.haildb.com/">HailDB</a> now supports ANALYZE for updating table stats</li>
	<li>drizzledump has added <a href="http://www.linuxjedi.co.uk/?p=87">--my-data-is-mangled</a> for handling certain MySQL charset migration issues</li>
	<li>SQLAlchemy dialect is now available for Drizzle (merged into<a href="http://www.sqlalchemy.org/"> SQLAlchemy</a> main)</li>
	<li>new experimental test-runner, <a href="http://www.wc220.com/?p=127">dbqp.py</a>, is in the tree for testing.  test-run.pl remains in the tree as our standby while development continues.</li>
	<li>migrated unittests to boost + additional work on expanding them and their usage.</li>
	<li>various updates to our <a href="http://docs.drizzle.org/">online documentation</a></li>
	<li>various other bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/+milestone/2011-01-31">here</a>
