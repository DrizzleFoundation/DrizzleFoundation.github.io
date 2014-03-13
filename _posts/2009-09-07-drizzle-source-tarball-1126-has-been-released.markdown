---
layout: post
status: publish
published: true
title: Drizzle source tarball 1126 has been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 327
wordpress_url: http://blog.drizzle.org/?p=327
date: 2009-09-07 13:29:14.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball based on build 1126 has been released. This marks the beginning of our march towards the Bell milestone in January.  In this release Monty added in support for automake 1.11. If automake 1.11 is used, then each line of the build will only produce a single short line of output, similar to builds of the Linux Kernel. Also like the Linux Kernel builds, the silent build mode can be disabled and the entire build line can be made visible again by adding V=1 to the invocation of make. Tarballs released from this point on will be generated using automake 1.11, so this behavior will be present in all tarballs.

The download file and change log can be found <a href="https://launchpad.net/drizzle/trunk/bell" target="_blank">here</a>

-Lee
