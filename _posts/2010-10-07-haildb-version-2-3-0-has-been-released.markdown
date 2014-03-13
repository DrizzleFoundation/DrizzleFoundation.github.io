---
layout: post
status: publish
published: true
title: HailDB version 2.3.0 has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 887
wordpress_url: http://blog.drizzle.org/?p=887
date: 2010-10-07 05:45:01.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
HailDB source tarball, version 2.3.0 has been released.

HailDB 2.3.0 - Athens release.

This is a Developer Release.

We have moved this release up to better align with the <a href="https://launchpad.net/drizzle/+milestone/2010-10-11">next Drizzle milestone</a>:
The Drizzle HailDB plugin for that release will require this version of HailDB

In this release:
<ul>
	<li>When hitting a constraint violation (duplicate key), HailDB returns which key was violated for more sensible error messages</li>
	<li>HailDB provides an API to table statistics</li>
	<li>HailDB now properly registered to use trx_is_interrupted, which determines if the currently running transaction has been interrupted</li>
	<li>Merged code from Innodb 1.0.7 as included in MySQL 5.1.46</li>
</ul>
The HailDB download file can be found <a href="https://launchpad.net/haildb/+milestone/athens">here</a>
