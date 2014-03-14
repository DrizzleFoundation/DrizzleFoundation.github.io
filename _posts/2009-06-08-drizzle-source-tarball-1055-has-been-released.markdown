---
layout: post
status: publish
published: true
title: Drizzle source tarball 1055 has been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 87
wordpress_url: http://blog.drizzle.org/?p=87
date: 2009-06-08 12:49:46.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball based on build 1055 has now been released. The change log can be viewed at https://launchpad.net/drizzle/trunk/aloha. 

For this release we continue to focus on code clean up, build improvements, increased test coverage and performance improvements. We also removed LOCK TABLES, BIT_COUNT and BIT_LENGTH, made several logging improvements, started the first several phases of refactoring JOIN and provided initial support for gcc 4.4 although for now you still need <a href="https://lists.launchpad.net/drizzle-discuss/msg04208.html">Monty's patch</a> for protobuf to use gcc 4.4. 

-Lee


