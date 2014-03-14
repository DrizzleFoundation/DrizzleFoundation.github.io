---
layout: post
status: publish
published: true
title: Drizzle build 1240 and libdrizzle 0.6 source tarballs have been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 435
wordpress_url: http://blog.drizzle.org/?p=435
date: 2009-12-08 10:49:59.000000000 +00:00
categories:
- Release
tags: []
comments: []
---
For Drizzle build 1240 this release includes:  
	<li>Dynamic loading of plugins at server start up</li>
	<ul><li>The majority of the existing plugins have been set to be loaded dynamically rather than compiled statically with the server </li></ul>
	<ul>
<li>Non-default plugin modules can be loaded with a command line option, ---plugin-add, which takes a comma-separated list of plugin module names, e.g.: ---plugin-add=csv,memcached_functions</li></ul>
	<ul>
<li>---plugin-add will load the default list of plugins in addition to the plugins requested</li></ul>
	<ul>
<li>---plugin-load which takes a similar list but overrides the entire list of plugins to be loaded</li></ul>
        <ul>
<li>In the source tree plugin test cases are now kept with the plugins themselves, so a provided plugin can be self-contained and also provide test cases</li></ul>
	<li>HEAP has been renamed to MEMORY when specifying the storage engine</li>
	<li>The Drizzle download file and change log can be found <a href="https://launchpad.net/drizzle/trunk/bell" target="_blank">here</a></li>


For libdrizzle version 0.6 this release includes:
	<li>Various cleanup and fixes around custom socket event handling and listening code</li>
	<li>Updated autoconf build system</li>
	<li>Updated RPM packaging</li>
	<li>The libdrizzle download file and change log can be found <a href="https://launchpad.net/libdrizzle/trunk/0.6" target="_blank">here</a></li>
	<li>Documentation for libdrizzle can be found at <a href="http://drizzle.org/libdrizzle-doxygen-api/modules.html"  target="_blank">API </a> and <a href="http://drizzle.org/libdrizzle-doxygen-dev/modules.html" target="_blank">Development</a></li>
