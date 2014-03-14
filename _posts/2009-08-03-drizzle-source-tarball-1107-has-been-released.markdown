---
layout: post
status: publish
published: true
title: Drizzle source tarball 1107 has been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 281
wordpress_url: http://blog.drizzle.org/?p=281
date: 2009-08-03 17:59:46.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
Drizzle source tarball based on build 1107 has been released. The big item for this release is Jay's initial work on replication. This first release includes a default simple replicator plugin and a command log plugin, which logs all changes to the server in a log file containing <a href="http://code.google.com/apis/protocolbuffers/">Google Protobuffer</a> command messages. The command log is used by other replication-focused modules which will be featured in the upcoming Aloha and Bell releases and forms the basis of standardized communication about changes to a server's data.

The download file and change log can be found <a href="https://launchpad.net/drizzle/trunk/aloha">here</a>  
