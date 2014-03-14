---
layout: post
status: publish
published: true
title: sqlbench now part of Drizzle testing framework
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 310
wordpress_url: http://blog.drizzle.org/?p=310
date: 2009-08-24 09:54:41.000000000 +00:00
categories:
- This Week In Drizzle
tags: []
comments: []
---
Thanks to <a href="http://capttofu.livejournal.com/" target="_blank">Patrick Galbraith</a> we now have <a href="https://launchpad.net/sql-bench" target="_blank">sqlbench</a> running and thanks to <a href="http://jpipes.com/" target="_blank">Jay's</a> guidance also have it integrated into the <a href="https://launchpad.net/drizzle-automation" target="_blank">Drizzle Automation</a> framework. We have added sqlbench as a job in our <a href="http://gorf.tangent.org/hudson/view/Drizzle/job/Drizzle-sql-bench-staging/" target="_blank">Hudson</a> framework so that it will now automatically run every time there are updates to the staging branch.  If you want to be on the email list for receiving any of the benchmark results, please register <a href=" https://launchpad.net/~drizzle-benchmark" target="_blank">here</a>.

Next up, crash-me which is currently running but needs some polish before we declare success.

-Lee
