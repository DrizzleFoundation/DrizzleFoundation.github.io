---
layout: post
status: publish
published: true
title: HailDB version 2.1.0 has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 850
wordpress_url: http://blog.drizzle.org/?p=850
date: 2010-09-21 13:07:51.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
HailDB source tarball, version 2.1.0 has been released.

NOTE:  This release was delayed slightly to resolve some last-minute build issues

In this release:
<ul>
	<li> ib_status_get_all - like ib_cfg_get_all (which gets a list of all  configuration names available to get/set), but for status variables</li>
	<li>updated pandora-build to 0.141</li>
	<li> removed UNIV_STATIC, which is no longer used in the innodb plugin either</li>
	<li>removed WITH_ZIP</li>
</ul>
The HailDB download file can be found <a href="https://launchpad.net/haildb/2.x/2.1">here</a>
