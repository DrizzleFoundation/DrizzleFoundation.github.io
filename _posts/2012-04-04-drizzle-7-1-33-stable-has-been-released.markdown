---
layout: post
status: publish
published: true
title: Drizzle 7.1.33-stable has been released
author: Vijay Samuel
author_login: vjsamuel
author_email: vjsamuel1990@gmail.com
wordpress_id: 1252
wordpress_url: http://blog.drizzle.org/?p=1252
date: 2012-04-04 07:25:44.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 235
  author: Drizzle 7.1.33-stable has been released &laquo; async I/O News
  author_email: ''
  author_url: http://asyncionews.com/?p=1350
  date: '2012-04-04 22:37:53 +0000'
  date_gmt: '2012-04-05 06:37:53 +0000'
  content: '[...] Read full article  Tagged as: DB, Drizzle, InnoDB, MySQL, RDBMS,
    SQL Comments Off     Comments (0) Trackbacks (0) ( subscribe to comments on this
    post ) [...] '
- id: 236
  author: Drizzle 7.1 released at Hack Drizzle
  author_email: ''
  author_url: http://hackdrizzle.com/drizzle-7-1-released/
  date: '2012-04-06 15:57:47 +0000'
  date_gmt: '2012-04-06 23:57:47 +0000'
  content: '[...] Drizzle 7.1 has been released.  In my frank opinion, there&#8217;s
    no longer any reason to use 7.0; everyone should upgrade to 7.1 because it is
    far superior.  Read the release announce for the list of new and fixed things.
     Most importantly, imho: sweeping updates to docs.drizzle.org.  This is also good
    news because in a few days I&#8217;m giving a presentation, Getting Started with
    Drizzle 7.1. [...] '
- id: 238
  author: '&raquo; Percona welcomes Drizzle 7.1 Pablo Gallego Falcón'
  author_email: ''
  author_url: http://pablo.gallegofalcon.com/?p=453
  date: '2012-04-10 09:14:00 +0000'
  date_gmt: '2012-04-10 17:14:00 +0000'
  content: '[...] Drizzle team has published the first Drizzle 7.1 stable release.
    The announcement on the Drizzle blog covers some of the major improvements in
    this release over the previous stable release, Drizzle [...] '
- id: 240
  author: Percona welcomes Drizzle 7.1 - MySQL Performance Blog
  author_email: ''
  author_url: http://www.mysqlperformanceblog.com/2012/04/10/percona-welcomes-drizzle-7-1/
  date: '2012-04-18 00:10:22 +0000'
  date_gmt: '2012-04-18 08:10:22 +0000'
  content: '[...] Drizzle team has published the first Drizzle 7.1 stable release.
    The announcement on the Drizzle blog covers some of the major improvements in
    this release over the previous stable release, Drizzle [...] '
- id: 243
  author: Ahmed Medhat
  author_email: ultimatetux@gmail.com
  author_url: http://-
  date: '2012-05-15 19:28:34 +0000'
  date_gmt: '2012-05-16 03:28:34 +0000'
  content: Good news, Though it seems the 7.1 root dir is not available from within
    http://download.drizzle.org/7.1/ or is it just me ?!
---
The Global Drizzle Development Team is pleased to announce the immediate availability of Drizzle 7.1.33-stable. The first stable release of Drizzle 7.1 and the result of 12 months of hard work from contributors around the world.

<strong>Improvements in Drizzle 7.1 compared to 7.0</strong>

- Xtrabackup is included (in-tree) by <a href="http://flamingspork.com/" target="_blank">Stewart Smith</a>

- Multi-source replication by <a href="http://dshrewsbury.blogspot.in/" target="_blank">David Shrewsbury</a>
<div>- Improved execute parser by <a href="http://blog.krow.net/" target="_blank">Brian Aker</a> and <span style="color: #888888;"><a href="http://vjsamuel.wordpress.com/" target="_blank">Vijay Samuel</a> </span></div>
<div>- Servers are identified with UUID in replication by <span style="color: #888888;"><a href="http://www.8bitsofbytes.com/" target="_blank">Joe Daly</a></span></div>
- HTTP JSON API (experimental) by <a href="http://flamingspork.com/" target="_blank">Stewart Smith</a>

- Percona Innodb patches merged by <a href="http://www.percona.com/about-us/our-team/laurynas-biveinis/" target="_blank">Laurynas Biveinis</a>

- JS plugin: execute JavaScript code as a Drizzle function by <a href="http://openlife.cc/" target="_blank">Henrik Ingo</a>

- IPV6 data type by Muhammad Umair

- Improvements to libdrizzle client library by <a href="http://linuxjedi.co.uk/" target="_blank">Andrew Hutchings</a> and <a href="http://blog.krow.net/" target="_blank">Brian Aker</a>

- Query log plugin and auth_schema by <a href="http://hackdrizzle.com/" target="_blank">Daniel Nichter</a>

- ZeroMQ plugin by <a href="http://developian.blogspot.in/" target="_blank">Markus Eriksson</a>

- Ability to publish transactions to zeromq and rabbitmq by <a href="http://developian.blogspot.com/" target="_blank">Marcus Eriksson</a>

- Replication Dictionary by <a href="http://blog.krow.net/" target="_blank">Brian Aker</a>

- Log output to syslog is enabled by default by <a href="http://blog.krow.net/" target="_blank">Brian Aker</a>

- Improvements to logging stats plugin

- Removal of drizzleadmin utility (you can now do all administration from drizzle client itself) by <a href="http://www.linuxjedi.co.uk/" target="_blank">Andrew Hutchings</a>

- Improved Regex Plugin by <span style="color: #888888;"><a href="http://fewbar.com/" target="_blank">Clint Byrum</a></span>

- Improvements to pandora build by <a href="http://www.inaugust.com/" target="_blank">Monty Taylor</a>

- New version numbering system and support for it in pandora-build by <a href="http://openlife.cc/" target="_blank">Henrik Ingo</a>

- Updated DEB and RPM packages, by <a href="http://openlife.cc/" target="_blank">Henrik Ingo</a>

- Revamped testing system Kewpie all-inclusive with suites of randgen, sysbench, sql-bench, and crashme tests by <a href="http://www.wc220.com/" target="_blank">Patrick Crews</a>

- Removal of HailDB engine by <a href="http://flamingspork.com/" target="_blank">Stewart Smith</a>

- Removal of PBMS engine

- Continued code refactoring by Olaf van der Spek, <a href="http://blog.krow.net/" target="_blank">Brian Aker</a> and others

- many bug fixes

<a href="http://blog.krow.net/" target="_blank">Brian Aker</a> ,<a href="http://mark.atwood.name/" target="_blank">Mark Atwood</a>- Continuous Integration

<a href="http://vjsamuel.wordpress.com/" target="_blank">Vijay Samuel</a> - Release Manager

<strong>Installing Drizzle 7.1.33-stable</strong>

The source tar package is available from our<a href="https://launchpad.net/drizzle/+milestone/7.1.33"> Launchpad download area</a>.<strong> </strong><a href="http://docs.drizzle.org/installing/from_source.html" target="_blank">Please see the manual on how to install Drizzle 7.1.33-stable from source tar package.</a>

The Ubuntu packages are available from the <a href="https://launchpad.net/%7Edrizzle-developers/+archive/ppa" target="_blank">Drizzle PPA</a>. Instructions on <a href="http://docs.drizzle.org/installing/ubuntu.html" target="_blank">how to install from the PPA are in the Drizzle manual</a>.

CentOS 6 packages are available from <a href="http://download.drizzle.org/7.1/" target="_blank">download.drizzle.org</a>. <a href="http://docs.drizzle.org/installing/redhat.html" target="_blank">Instructions on how to install them with yum are in the Drizzle manual.</a>

Note: For Drizzle 7.1.33-stable, only 64-bit packages were built for RedHat/Centos.

<strong>Known issues</strong>

All of the optional plugins are packaged in their own package. These are named drizzle-plugin-*. If a plugin is installed, it is also configured to load by default. (see /etc/drizzle/conf.d/pluginname.cnf) However, not all plugins actually work without further configuration. These plugins will cause the server startup to fail. The workaround is to either configure the plugin to work, or uninstall it if you don't want to use it. (<a href="https://blueprints.launchpad.net/drizzle/+spec/plugin-standards" target="_blank">Related blueprint</a>) In short, you should only install the plugins you want to use. Don't install all available plugins. You also need to use "yum erase" and "apt-get purge" to uninstall plugins.
<div>

Please post bugs on the <a href="https://bugs.launchpad.net/drizzle" target="_blank">Drizzle bug tracker</a> and questions and general feedback to <a href="https://launchpad.net/%7Edrizzle-discuss/" target="_blank">drizzle-discuss mailing list</a>.

</div>
<strong>Drizzle documentation</strong>

Much improved documentation is available at <a href="http://docs.drizzle.org/" target="_blank">docs.drizzle.org</a>

<strong>Planet Drizzle</strong>

You can follow our developer blogs, with more information about the features in Drizzle 7.1 at <a href="http://planetdrizzle.org/" target="_blank">planetdrizzle.org</a>
<div>

<strong>Percona Live MySQL Conference and Drizzle Day</strong>

The Drizzle team will be well represented at next week's <a href="http://www.percona.com/live/mysql-conference-2012/" target="_blank">Percona Live MySQL Conference</a> and Expo and the <a href="http://www.drizzle.org/content/drizzle-day-fri-13-apr-2012-santa-clara" target="_blank">Drizzle Day</a> in the Santa Clara Convention Center. There are a couple talks from Drizzle developers and users in the main conference, and a full day on Friday, Apr 13. Drizzle Day is free to attend (though donations are encouraged). Please join us in Santa Clara and come and say hi!

&nbsp;

</div>
<div>

<strong>Commercial 24/7 support is available</strong>

Several support vendors in the MySQL space provide commercial support and services for Drizzle 7.1. <a href="http://www.drizzle.org/content/support-and-services" target="_blank">Click here</a> for a list of support vendors that contributed to Drizzle during the 7.1 release cycle.

</div>
<div>

<strong>Info to press</strong>

Drizzle core developers are available for email and phone interviews to discuss Drizzle 7.1 and also upcoming Drizzle topics. To arrange an interview, please contact

</div>
In Americas: Brian Aker <a href="mailto:brian@tangent.org%20" target="_blank">brian@tangent.org</a>,  Mark Atwood <a href="mailto:me@mark.atwood.name" target="_blank">me@mark.atwood.name</a>, Kent Bozlinski : <a href="mailto:kent@bozlinski.com" target="_blank">kent@bozlinski.com</a>

In EMEA: Henrik Ingo <a href="mailto:henrik.ingo@avoinelama.fi" target="_blank">henrik.ingo@avoinelama.fi</a>
<div>In APAC: Stewart Smith <a href="mailto:stewart.smith@percona.com" target="_blank">stewart.smith@percona.com</a></div>
&nbsp;
