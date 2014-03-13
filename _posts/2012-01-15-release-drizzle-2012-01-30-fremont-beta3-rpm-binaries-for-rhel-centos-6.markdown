---
layout: post
status: publish
published: true
title: 'Release: Drizzle 2012.01.30 (Fremont beta3) RPM binaries for RHEL / CentOS
  6'
author: Henrik Ingo
author_login: henrik
author_email: henrik.ingo@avoinelama.fi
wordpress_id: 1219
wordpress_url: http://blog.drizzle.org/?p=1219
date: 2012-01-15 13:12:18.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 216
  author: 'Release: Drizzle 2012.01.30 (Fremont beta3) RPM &#8230; &#8211; drizzle.org'
  author_email: ''
  author_url: http://rpm47.com/2012/01/release-drizzle-2012-01-30-fremont-beta3-rpm-drizzle-org/
  date: '2012-01-15 15:30:12 +0000'
  date_gmt: '2012-01-15 23:30:12 +0000'
  content: '[...] the article here: Release: Drizzle 2012.01.30 (Fremont beta3) RPM
    &#8230; &#8211; drizzle.org Please check out our sister sites! Home pay Buyer
    pay Interest pay Fee pay New pay Childbirth [...] '
- id: 218
  author: 'Making rpm builds a first class citizen: Why? | OpenLife.cc'
  author_email: ''
  author_url: http://openlife.cc/blogs/2012/january/making-rpm-builds-first-class-citizen-why
  date: '2012-01-19 14:50:28 +0000'
  date_gmt: '2012-01-19 22:50:28 +0000'
  content: '[...]  Last weekend I released rpm files for the latest Drizzle Fremont
    beta (announcement). As part of that work I&#039;ve also integrated the spec file
    and other files used by the rpmbuild into [...] '
- id: 221
  author: Evan
  author_email: evan@shipwire.com
  author_url: ''
  date: '2012-02-14 09:32:34 +0000'
  date_gmt: '2012-02-14 17:32:34 +0000'
  content: Forgive me if this was mentioned elsewhere, but are you planning to build
    RPMs for CentOS 5 as well?
- id: 222
  author: Henrik Ingo
  author_email: henrik.ingo@avoinelama.fi
  author_url: http://openlife.cc/
  date: '2012-02-14 12:04:52 +0000'
  date_gmt: '2012-02-14 20:04:52 +0000'
  content: |-
    Ah, good question!

    So it should be pointed out that Drizzle 7 release does already come with both RPMs and DEBs, including (of course) for CentOS 5. See http://docs.drizzle.org/installing/redhat.html

    Otoh it seems the upcoming Drizzle 7.1 doesn't build on CentOS 5 anymore, nor is there any interest to support it as far as I know.
---
<div id="release-notes">

Hot on the heels of this week's Drizzle 2012.01.30 source release, we are now also releasing beta quality binary RPMs for your downloading and testing pleasure! While we are revitalizing the Drizzle yum repository, you can download the rpm-bundle from our Launchpad project page: <a title="Drizzle DEB and RPM downloads" href="https://launchpad.net/pkg-drizzle/+download">https://launchpad.net/pkg-drizzle/+download</a>

As the Fremont development cycle is ending it's beta cycle and heading for release candidates, we are starting to publish also binary packages for downloads. Today we are releasing RPM packages for RHEL/CentOS 6.0. Fedora 16 packaging has unfortunately been postponed. We will eventually support also Fedora 16 RPMs, but in the mean time you can possibly spot some Drizzle developers on twitter or irc making snarky comments about systemd ...

In the following week(s) we will also publish Debian and Ubuntu packages.

Note that these packages are a first release of their kind and still a bit experimental. What this means is that the underlying Drizzle release itself is stabilizing quite nicely, but the packaging process is currently not completely integrated nor automated.

Please report errors at <a title="Drizzle bug tracker" href="https://bugs.launchpad.net/drizzle">the main Drizzle bug tracker</a>, and direct your general feedback to the <a href="https://launchpad.net/~drizzle-discuss">drizzle-discuss mailing list</a>.

<strong>Details:</strong>
<ul>
	<li>These packages were built from the Drizzle bzr trunk at tag 2012.01.30.</li>
	<li>In addition a branch that supports "make rpm" was merged from <a href="https://launchpad.net/+branch/%7Ehingo/drizzle/drizzle-integrate-packaging-rpm">lp:~hingo/drizzle/drizzle-integrate-packaging-rpm</a>. This is based on the same RPM spec as was used for Drizzle 7, but the intent is to integrate it with the main Drizzle source code and then Jenkins builds. The current release was however still a manual process.</li>
	<li>When building this way, an additional bzr tag --force 2012.01.30 was needed to maintain the same version number.</li>
	<li>Along the RPMs we have uploaded a source tar file fake-drizzle7-<wbr>2012.01.<wbr>30.tar.<wbr>gz. This corresponds to the real Drizzle 2012.01.30 release, plus the above changes.</wbr></wbr></wbr></li>
	<li>The RPM files are made available as a tar bundle. The process to publish into the Drizzle yum repository is currently broken but will resume in the near future.</li>
	<li>A related issue is that the packages are not signed.</li>
	<li>Known issue: If you install the plugin rpms, they will be automatically loaded at startup. However, some of them (in particular, many auth plugins, the policy plugins and possibly the slave plugin) don't actually work without further configuration and will thus prevent the server from starting. If you encounter this plugin, you should either complete the configuration (in /etc/drizzle/conf.d/[plugin].conf) or, if you don't want to use it, uninstall the plugin.</li>
</ul>
</div>
