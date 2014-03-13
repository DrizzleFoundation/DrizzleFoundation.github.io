---
layout: post
status: publish
published: true
title: Drizzle now running dbt2 benchmark
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 481
wordpress_url: http://blog.drizzle.org/?p=481
date: 2009-12-31 09:19:57.000000000 +00:00
categories:
- This Week In Drizzle
tags: []
comments: []
---
We recently added support for running the <a href="http://git.postgresql.org/gitweb?p=dbt2.git">dbt2</a> benchmark as part of our <a href="http://drizzle.org/wiki/Automation_Documentation">drizzle automation</a> suite. dbt2 is an OLTP transactional performance test. It simulates a wholesale parts supplier where several workers access a database, update customer information and check on parts inventories. We currently are using the defaults (10 warehouses, 5 minute test runs and running various number of connections for each run up to 1024. The initial runs exposed a <a href="https://bugs.launchpad.net/drizzle/+bug/500031">race condition</a> in our TemporalFormat::match() code at 1024 connections.

We now have a very nice suite of tools to help us with tracking performance and scalability of Drizzle, besides dbt2 we also are running sysbench, sqlbench, crash-me and randgen for all of our builds in the <a href="http://hudson.drizzle.org/view/Drizzle-staging/">staging branch</a> of Drizzle. Of course we are always looking for more, so if you have any suggestions on other benchmarks or tools to add, please let us know. 

If you want to receive all of the various benchmark results you can subscribe to the <a href="https://launchpad.net/~drizzle-benchmark">mailing list</a>.

Note also we are in the process of getting our changes to dbt2 merged to the dbt2 trunk, it should be there very soon.

Happy New Year to all!

-Lee
