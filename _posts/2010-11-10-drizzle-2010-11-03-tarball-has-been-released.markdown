---
layout: post
status: publish
published: true
title: Drizzle 2010.11.03 tarball has been released
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 924
wordpress_url: http://blog.drizzle.org/?p=924
date: 2010-11-10 11:46:47.000000000 +00:00
categories:
- Release
tags: []
comments:
- id: 55
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/11/10/drizzle-2010-11-03-tarball-has-been-released/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-11-10 13:54:07 +0000'
  date_gmt: '2010-11-10 21:54:07 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: PlanetDrizzle Official Drizzle Blog: Drizzle 2010.11.03 tarball
    has been released: Drizzle source tarball, versi... http://bit.ly/cxLktF [...] '
---
Drizzle source tarball, version 2010.11.03 has been released.
This is our 3rd beta release.  Many thanks to everyone who keeps downloading and using the software.  We've seen an uptick in downloads and bug reports since going beta.  Please keep the feedback coming : )

In this release:
<ul>
	<li>NEW DEPENDENCY - We now require libboost-iostreams-dev</li>
	<li>Drizzle now listens on port 4427 by default (clients use that port by default as well).  This allows for Drizzle and MySQL to run using their default ports on the same machine</li>
	<li> We now support the MySQL UNIX Socket protocol.  It is now possible to  connect to a Drizzle server with a mysql command line client via  sockets.  Start the server with the option --protocol-mysql-unix-socket.path=/tmp/mysql.sock.  You can then connect to the socket file via your mysql client.</li>
	<li> Added adjustable global upper cap for sort buffers.  This is to  limit the sum of all sort buffers across all running threads.  You can read more about this <a href="https://blueprints.launchpad.net/drizzle/+spec/limit-maximum-sort-size">here</a> and <a href="http://www.linuxjedi.co.uk/?p=47">here</a></li>
	<li> Added additional information to drizzleslap output to assist with bug diagnosis</li>
	<li> Automated randgen tests of the transaction log</li>
	<li> Added several additional options to the transaction_reader utility to help a user view the transaction log contents</li>
	<li> Work on removing locks from table shares</li>
	<li> Continued work on catalogs</li>
	<li> Continued work on documentation</li>
	<li> Continued code cleanup / refactoring</li>
	<li> 30 bug fixes</li>
</ul>
The Drizzle download file can be found <a href="https://launchpad.net/drizzle/elliott/2010-11-08">here</a>
