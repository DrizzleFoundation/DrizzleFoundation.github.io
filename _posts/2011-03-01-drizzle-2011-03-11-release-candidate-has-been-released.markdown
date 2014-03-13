---
layout: post
status: publish
published: true
title: Drizzle 2011.03.11 Release Candidate has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 1047
wordpress_url: http://blog.drizzle.org/?p=1047
date: 2011-03-01 09:41:46.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball, version 2011.03.11 has been released.  For those of you counting at home, that makes two...two RC's...ah ah hah! : )

While the original plan was to release a GA today, there are still some features we wanted to test more thoroughly before calling things good.  The plan is to have a GA release on 3/14.  The code is amazingly solid at this point and we feel confident in asking people to start to use it seriously.  Please help us test the heck out of <a href="http://drizzle.org/">Drizzle</a> to get ready for GA!

If you want the latest and greatest Drizzle news, we highly recommend LinuxJedi's <a href="http://www.linuxjedi.co.uk/?p=102">Last Week in Drizzle</a> feature.

Most of the work in this release has been polish, polish, and more polish as we near our first GA!

In this release:
<ul>
	<li>New native replication solution - the <a href="http://docs.drizzle.org/plugins/slave/index.html">slave plugin</a>!  This allows a Drizzle server to replicate from a master that is using the innodb replication log.  Read more about this <a href="http://dshrewsbury.blogspot.com/2011/02/drizzles-slave-plugin-and-execute-class.html">here</a> and <a href="http://www.wc220.com/?p=135">here</a></li>
	<li>Because you asked for it - MySQL BIT operators are back (thanks to <a href="http://krow.livejournal.com/">Brian Aker</a> for this)</li>
	<li>Continued work on system variables</li>
	<li>Continued work on catalogs</li>
	<li>Continued work on SQLAlchemy dialect / Drizzle interoperability</li>
	<li>Fixes for various performance regressions</li>
	<li>Continued work on <a href="http://docs.drizzle.org/">documentation</a></li>
	<li>random query generator integration with new test runner</li>
	<li>Over 30 bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2011-02-28">here</a>.
