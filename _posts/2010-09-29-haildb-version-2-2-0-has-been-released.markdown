---
layout: post
status: publish
published: true
title: HailDB version 2.2.0 has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 853
wordpress_url: http://blog.drizzle.org/?p=853
date: 2010-09-29 08:07:41.000000000 +00:00
categories:
- Uncategorized
- Release
tags: []
comments:
- id: 39
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/09/29/haildb-version-2-2-0-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-09-29 09:40:30 +0000'
  date_gmt: '2010-09-29 17:40:30 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog HailDB version 2.2.0 has been released: HailDB source
    tarball, version 2.1.0 has been released. In thi... http://bit.ly/b4lWiz [...] '
- id: 40
  author: HailDB 2.2.0 released! | HailDB
  author_email: ''
  author_url: http://www.haildb.com/2010/09/30/haildb-2-2-0-released/
  date: '2010-09-29 20:32:57 +0000'
  date_gmt: '2010-09-30 04:32:57 +0000'
  content: '[...] just released the 2.2.0 release! It was announced first on the Drizzle
    Blog last night. It&#8217;s a minor release, with some bug fixes since [...] '
---
HailDB source tarball, version 2.2.0 has been released.

In this release:

- Remove dict_table_check_for_dup_indexes(). It is now unneeded, there is a check in api/ for this, so embedded_innodb never had this problem.
- file_io_threads is deprecated but still exists - we now issue a warning about this if a user attempts to set it.
- fix of rmplint errors
- import fix for IMPORT TABLESPACE of compressed tables

The HailDB download file can be found <a href="https://launchpad.net/haildb/2.x/2.2">here</a>
