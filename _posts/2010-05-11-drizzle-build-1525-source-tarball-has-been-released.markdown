---
layout: post
status: publish
published: true
title: Drizzle build 1525 source tarball has been released
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 717
wordpress_url: http://blog.drizzle.org/?p=717
date: 2010-05-11 08:43:48.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 13
  author: BJ Dierkes
  author_email: wdierkes@5dollarwhitebox.org
  author_url: ''
  date: '2010-05-11 16:40:10 +0000'
  date_gmt: '2010-05-12 00:40:10 +0000'
  content: 'As a follow up to this, RPMs for RHEL 5 and Fedora 12 are also available
    via the unofficial drizzle repo.  Please see: http://drizzle.org/wiki/RPMInstallation
    .'
---
Drizzle source tarball based on build 1525 has been released. In this release:
<ul>
<li><a href="http://primebase.org/" target="_blank">pbxt</a> support is now available. To use the pbxt storage engine add  "--with-pbxt-plugin" during configuration and then add "--plugin_add=pbxt" when starting drizzled.</li>
<li>Eric added the OpenLDAP plugin, see his <a href="http://oddments.org/?p=349" target="_blank">blog</a> for details on writing Authentication plugins.</li>
<li>COM_STATS have been replaced with data from drizzle's internal scoreboard, thanks to Joe Daly for that contribution.</li>
</ul>

The Drizzle download file  can be found <a href="https://launchpad.net/drizzle/dexter/2010-05-10" target="_blank">here</a>.
