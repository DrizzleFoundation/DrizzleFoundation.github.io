---
layout: post
status: publish
published: true
title: Drizzle 2010.10.02 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 914
wordpress_url: http://blog.drizzle.org/?p=914
date: 2010-10-27 12:03:15.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 50
  author: Steffen
  author_email: steffen.weber@gmail.com
  author_url: ''
  date: '2010-10-27 14:20:59 +0000'
  date_gmt: '2010-10-27 22:20:59 +0000'
  content: What's the use-case for the EXECUTE functionality?
- id: 51
  author: Brian Aker
  author_email: brian@tangent.org
  author_url: http://krow.net/
  date: '2010-10-27 16:50:28 +0000'
  date_gmt: '2010-10-28 00:50:28 +0000'
  content: '@Steffen  EXECUTE is used for generating SQL in a dynamic manner on the
    server.'
- id: 52
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/10/27/drizzle-2010-10-02-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-10-27 18:15:09 +0000'
  date_gmt: '2010-10-28 02:15:09 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog Drizzle 2010.10.02 tarball has been released: Drizzle
    source tarball, version 2010.10.02 has been rele... http://bit.ly/b7clzV [...] '
- id: 53
  author: Steffen
  author_email: steffen.weber@gmail.com
  author_url: ''
  date: '2010-10-27 21:59:20 +0000'
  date_gmt: '2010-10-28 05:59:20 +0000'
  content: '@Brian: I can see this in the example above. But when is this useful?
    Sorry, I just can''t imagine where I would use it. :)'
- id: 54
  author: Brian Aker
  author_email: brian@tangent.org
  author_url: http://krow.net/
  date: '2010-10-28 10:55:11 +0000'
  date_gmt: '2010-10-28 18:55:11 +0000'
  content: |-
    @Steffen  For me I am using it for two purposes, the first is in test cases where I am selecting values inside of the database into variables, and then executing them from statements that I have already stored as variables (a binary SET operation from the client would make this a bit sharper, but that is a bit out of the scope of what I was needing at the time).

    The second thing I am using them for is to make sure that some of our work internally is allowing for re-entrance on the session level. Why? I've had a compile of Drizzle working with a perl interpreter internally just so that I can execute near the data (I don't expect to ever merge the perl bits BTW, I dislike having anything like perl that core to the kernel). I do want to make sure it continues to work though.
---
Drizzle source tarball, version 2010.10.02 has been released.

This is a beta-quality release.

Many thanks to everyone for the patches and bug reports.  Please keep them coming!

In this release:
<ul>
	<li>Added user locks</li>
	<li>Continued code cleanup and refactoring</li>
	<li>Removed two dead plugins (bad schedulers)</li>
	<li>Added documentation on replication</li>
	<li>Added options to the drizzled/messages/transaction_reader program, which allows us to convert transaction.log content into SQL: /path/to/transaction_reader path/to/transaction.log = SQL output of log contents.
We can now:
* view raw log ouput (rather than converted to SQL)
* view contents of the log from a specific message onward
* view the contents of a specific message</li>
	<li>Added UTF8 test cases for Tamil</li>
	<li>Added <a href="https://blueprints.launchpad.net/drizzle/+spec/add-execute">EXECUTE</a> functionality:
We can do:
* SET @VAR = "SELECT 1";
* EXECUTE @VAR;
* EXECUTE "SELECT 1";</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2010-10-25">here</a>
