---
layout: post
status: publish
published: true
title: 'Testing BlitzDB with the randgen. '
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 756
wordpress_url: http://blog.drizzle.org/?p=756
date: 2010-06-28 11:05:49.000000000 +00:00
categories:
- Uncategorized
tags: []
comments:
- id: 20
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/06/28/testing-blitzdb-with-the-randgen/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-06-28 12:35:10 +0000'
  date_gmt: '2010-06-28 20:35:10 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog Testing BlitzDB with the randgen.: Thanks to the
    hard work of Toru Maesaka, BlitzDB is now in Drizzle&#39;... http://bit.ly/cjFIKB
    [...] '
- id: 21
  author: Testing Drizzle with the random query generator | workcenter220
  author_email: ''
  author_url: http://www.wc220.com/?p=13
  date: '2010-08-06 07:50:32 +0000'
  date_gmt: '2010-08-06 15:50:32 +0000'
  content: '[...] At the time of this writing, 6 of these are in &#8216;Fix Released&#8217;
    status and 3 more are in work.  I&#8217;d like to extend a personal &#8220;Thank
    you&#8221; to Prafulla Tekawade for his great work &#8211; he has patches for
    5 out of the 6 fixed bugs (!).  Additionally, thanks for Toru Maesaka for his
    continued work on BlitzDB (which is part of our regular randgen testing). [...] '
---
<div id="_mcePaste">Thanks to the hard work of Toru Maesaka, <a href="https://launchpad.net/blitzdb">BlitzDB</a> is now in Drizzle's trunk.  As a result, we are now testing BlitzDB in our automated tests.</div><br>
<div id="_mcePaste">One of the easiest and most powerful ways of beating up on BlitzDB is via the <a href="https://launchpad.net/randgen">randgen</a> (RQG).  The RQG's data generation facility (gendata) is quite flexible and extensible and adding BlitzDB to the mix was very easy.  Beyond adding 'BlitzDB' to the engines section of the altered gendata files and adjusting / removing some data types to accommodate BlitzDB limitations, all that is required is for us to modify the grammars to accomodate any changes to the test tables.</div><br>
<div id="_mcePaste">This new setup provides us with a test bed of both Innodb and BlitzDB tables and queries that will mix the different tables.  Of course, we still keep the original tests to provide even more testing for Innodb only.</div><br>
<div id="_mcePaste">We now have 4 tests that utilize BlitzDB in our automated testing:</div>
<div id="_mcePaste">
<ul>
	<li>optimizer_subquery_mix_engine</li>
	<li>optimizer_subquery_mix_engine_rand</li>
	<li>outer_join_mix_engine</li>
	<li>outer_join_mix_engine_rand</li>
</ul>
</div><br>
<div>The grammars and gendata files have been pushed to lp:randgen and the tests are part of drizzle-automation's randgen testing.</div><br>
<div id="_mcePaste">These tests are based on two of the most productive RQG grammars we have.  The 'mix' suffix means that we are mixing different storage engines across queries (we will likely add additional storage engines over time - looking at you, <a href="http://www.primebase.org/">PBXT</a>).  <br><br>The 'rand' tests make use of the RQG's '--seed' option for increased randomness.  For a given seed value, the queries and generated data will be consistent on any machine.  By using seed=time in certain tests, we guarantee that we are constantly trying new data and query combinations in addition to our standard tests.</div><br>
<div id="_mcePaste">Additional information regarding Drizzle testing (including the randgen) can be found <a href="http://drizzle.org/wiki/DrizzleQA">here</a>.  Please feel free to make use of the mailing lists if you want to get involved, have questions, etc - there's plenty of work for anyone who is interested : )</div>
