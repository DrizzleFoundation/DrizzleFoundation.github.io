---
layout: post
status: publish
published: true
title: Drizzle 2011.01.07 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 956
wordpress_url: http://blog.drizzle.org/?p=956
date: 2011-01-04 07:46:00.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball, version 2010.01.07 beta has been released.  This is the first Drizzle release of 2011 (aka the <a href="http://www.linuxjedi.co.uk/?p=65">year of Drizzle</a>!).

In this release:
<ul>
	<li>Clean up of drizzled command line options</li>
	<li>Refactored drizzleslap code - thanks to <a href="http://vjsamuel.wordpress.com/">Vijay Samuel</a> for tackling this : )</li>
	<li>Updated innobase plugin to be based on innodb 1.1.4 from MySQL 5.5.8</li>
	<li>All timers in Drizzle have been updated to be microsecond internally</li>
	<li>New TIME data type</li>
	<li>New BOOLEAN data type (storage is engine-dependent)</li>
	<li>New assert() function.  Evaluates an expression and errors out based on true/{false/NULL}</li>
	<li>New typeof() function.  Evaluates an expression and returns our internal type</li>
	<li>New result_type() function.  Returns the internal result type that is being used (ie STRING, INT, DECIMAL,...)</li>
	<li>updates to storage engine api and testing tool</li>
	<li>continued work on transaction log code</li>
	<li>various bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2011-01-03">here</a>
