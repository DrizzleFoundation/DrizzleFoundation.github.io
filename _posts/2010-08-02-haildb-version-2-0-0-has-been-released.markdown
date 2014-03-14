---
layout: post
status: publish
published: true
title: HailDB version 2.0.0 has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 808
wordpress_url: http://blog.drizzle.org/?p=808
date: 2010-08-02 16:49:56.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
HailDB source tarball, version 2.0.0 has been released.
In this version:
- A lot of compiler warnings have been fixed.
- The build system is now pandora-build.
- some small bugs have been fixed
- Header file is now haildb.h instead of innodb.h
- We display "HailDB" instead of "Embedded InnoDB"
- Library name is libhaildb instead of libinnodb
- It is probably binary compatible with the last Embedded InnoDB release, but we don't have explicit tests for that, so YMMV

The HailDB download file can be found [https://launchpad.net/haildb/+milestone/release-2.0 here] 
