---
layout: post
status: publish
published: true
title: Drizzle build 1347 and libdrizzle 0.8 source tarballs have been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 616
wordpress_url: http://blog.drizzle.org/?p=616
date: 2010-03-17 11:30:12.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
For Drizzle build 1347 this includes: 
<li> Brian's implementation of the <a href="http://krow.livejournal.com/685840.html" target="_blank">Data Dictionary</a> work which temporarily removes Information Schema. Look for an ANSI compliant Information Schema to be back in our next release in two weeks.</li>  
<li>Switched the default protocol to use the MySQL protocol. See <a href="http://oddments.org/?p=307" target="_blank">Eric's blog </a>for a great summary and details.   Note that as of today the <a href="https://launchpad.net/drizzle-jdbc" target="_blank">Drizzle JDBC driver</a> will not work, however Marcus is working on it and should have a fix very soon.</li>
<li>The Drizzle download file and change log can be found <a href="https://launchpad.net/drizzle/cherry/2010-03-15" target="_blank">here</a></li>

For libdrizzle build 0.8 this release includes:
	<li>Added prototest suite for testing the MySQL protocol</li>
        <li>Changed default protocol to be MySQL for Drizzle connections to stay in sync with defaults on the Drizzle server</li>
        <li>Build system and RPM packaging updates</li>
        <li>Bug fixes in concurrent query execution and compiling for FreeBSD</li>
	<li>The libdrizzle download file and change log can be found <a href="https://launchpad.net/libdrizzle/trunk/0.8" target="_blank">here</a></li>
	<li>Documentation for libdrizzle can be found at <a href="http://drizzle.org/libdrizzle-doxygen-api/modules.html"  target="_blank">API </a> and <a href="http://drizzle.org/libdrizzle-doxygen-dev/modules.html" target="_blank">Development</a></li>
