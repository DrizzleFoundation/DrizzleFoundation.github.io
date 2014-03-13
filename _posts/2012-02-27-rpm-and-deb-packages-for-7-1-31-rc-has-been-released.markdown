---
layout: post
status: publish
published: true
title: RPM and DEB packages for 7.1.31-rc has been released
author: Henrik Ingo
author_login: henrik
author_email: henrik.ingo@avoinelama.fi
wordpress_id: 1231
wordpress_url: http://blog.drizzle.org/?p=1231
date: 2012-02-27 13:34:26.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 228
  author: Drizzle versions and RPM deficiencies | OpenLife.cc
  author_email: ''
  author_url: http://openlife.cc/blogs/2012/february/drizzle-versions-and-rpm-deficiencies
  date: '2012-02-28 04:46:06 +0000'
  date_gmt: '2012-02-28 12:46:06 +0000'
  content: '[...] and RPM deficiencies     Submitted by hingo on Tue, 2012-02-28 11:48
    Drizzle  Yesterday I released RPM and DEB packages for the Drizzle 7.1.31-rc Release
    Candidate. This was the first Drizzle release featuring what I like to call &quot;sane
    versioning number&quot;. Here I [...] '
---
The first <a href="http://blog.drizzle.org/2012/02/15/drizzle-7-1-release-candidate-1-7-1-31-rc-has-been-released/">Drizzle 7.1 Release Candidate was released 2 weeks ago</a>. It contained a few last minute changes that broke the packaging process (version number and decision to package libdrizzle separately) and hence only a source release was made. However, we are happy to announce that we have now caught up with those changes and binary packages are today available for RHEL/Centos 6 and Ubuntu 11.10 Oneiric.

In addition we are working closely with the Debian project to upload Drizzle 7.1.x into Debian unstable repository in the near future. This will be the primary place to get Drizzle for Debian and we will not be setting up any other Debian repository ourselves. As of today you can already find the stable Drizzle 7 release in Debian unstable. Thanks to Tobias Frost for stepping up as the Drizzle packager for Debian.

Fedora packages were not provided at this time. This is due to Fedora 16 switching to the new systemd, which rendered our standard init script unusable. We will probably look into systemd startup scripts at some point in the future.

<strong>Installing Drizzle 7.1.31-rc on Ubuntu.</strong>

The Ubuntu packages are available from the <a href="https://launchpad.net/~drizzle-developers/+archive/ppa">Drizzle PPA</a>. Instructions on <a href="http://docs.drizzle.org/installing/ubuntu.html">how to install from the PPA are already in the Drizzle manual</a>.

<strong>Installing Drizzle 7.1.31-rc on RedHat / Centos 6.</strong>

Note: For Drizzle 7.1.31-rc, only 64-bit packages were built for RedHat/Centos. Please let us know if there is demand for 32-bit packages (such as commenting to this blog post.)

A pre-requisite is to install the EPEL repository:
<pre title="">su -c 'rpm -ivh http://download.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-5.noarch.rpm'</pre>
After this, please add the following to /etc/yum.repos.d/drizzle.repo
<pre title="">   [drizzle]
   name=drizzle
   baseurl=http://download.drizzle.org/7.1/redhat/$releasever/$basearch/
   enabled=1
   gpgcheck=0

   [drizzle-src]
   name=drizzle-src
   baseurl=http://download.drizzle.org/7.1/redhat/$releasever/source
   enabled=1
   gpgcheck=0</pre>
Note that the baseurl is different from what was used for Drizzle 7.

<strong>Known issues</strong>

All of the optional plugins are packaged in their own package. These are named drizzle-plugin-*. If a plugin is installed, it is also configured to load by default. (see /etc/drizzle/conf.d/pluginname.cnf) However, not all plugins actually work without further configuration. These plugins will cause the server startup to fail. The workaround is to either configure the plugin to work, or uninstall it if you don't want to use it. (<a href="https://blueprints.launchpad.net/drizzle/+spec/plugin-standards">Related blueprint</a>) In short, you should only install the plugins you want to use. Don't install all available plugins.

<strong>Resources</strong>

To know what's new in this release, you can <a href="http://blog.drizzle.org/2012/02/15/drizzle-7-1-release-candidate-1-7-1-31-rc-has-been-released/">read the 7.1.31-rc release notes here</a>.<strong></strong> Please post bugs on the <a href="https://bugs.launchpad.net/drizzle">Drizzle bug tracker</a> and questions and general feedback to <a href="https://launchpad.net/~drizzle-discuss/">drizzle-discuss mailing list</a>.
