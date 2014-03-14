---
layout: post
status: publish
published: true
title: 'Testing Drizzle''s transaction log '
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 783
wordpress_url: http://blog.drizzle.org/?p=783
date: 2010-07-09 14:12:48.000000000 +00:00
categories:
- Uncategorized
tags:
- Drizzle
- replication
- testing
comments:
- id: 23
  author: Tweets that mention drizzle.org -- Topsy.com
  author_email: ''
  author_url: http://topsy.com/blog.drizzle.org/2010/07/09/testing-drizzles-transaction-log/?utm_source=pingback&amp;utm_campaign=L2
  date: '2010-07-09 15:27:30 +0000'
  date_gmt: '2010-07-09 23:27:30 +0000'
  content: '[...] This post was mentioned on Twitter by drizzlenews, drizzlenews.
    drizzlenews said: DrizzleBlog Testing Drizzle&#39;s transaction log: One of my
    first tasks on the Drizzle team was to check out the tran... http://bit.ly/aEWn2u
    [...] '
- id: 24
  author: Stewart Smith
  author_email: stewart@flamingspork.com
  author_url: http://www.flamingspork.com/blog/
  date: '2010-07-09 21:13:36 +0000'
  date_gmt: '2010-07-10 05:13:36 +0000'
  content: I'm working on the FOREIGN KEY bug. It's going to get done along with SHOW
    CREATE TABLE using the same code path as the replication code (statement_transform)
    so we'll have a much higher likelihood of it being correct.
- id: 25
  author: Evolution of the AS400 and ISeries-business
  author_email: ''
  author_url: http://www.3business.info/evolution-of-the-as400-and-iseries.html
  date: '2010-08-12 09:22:23 +0000'
  date_gmt: '2010-08-12 17:22:23 +0000'
  content: '[...] Testing Drizzle&#39;s transaction log &#8211; drizzle.org [...] '
- id: 26
  author: Basic replication from Drizzle&#8217;s transaction log now being tested.
    | workcenter220
  author_email: ''
  author_url: http://www.wc220.com/?p=58
  date: '2010-09-23 09:02:16 +0000'
  date_gmt: '2010-09-23 17:02:16 +0000'
  content: '[...] I wrote earlier, we have already spent some time on basic tests
    of the transaction log structure &#8211; i.e. can [...] '
---
<div id="_mcePaste">One of my first tasks on the Drizzle team was to check out the transaction log, part of <a href="http://www.joinfu.com/">Jay Pipes'</a> work on replication.  We needed to make sure that the log itself was rock-solid and that any code written to use it would have a worthy foundation.  As it turns out, some people are really interested in getting replication working ; )</div></br></br>

<div id="_mcePaste">As can be seen from the <a href="https://blueprints.launchpad.net/drizzle/+spec/test-transaction-log">blueprint</a>, testing will involve two of our main testing tools, the randgen and our standard test suite (test-run, dtr, etc).  So far, our efforts have been concentrated on writing tests for the test suite.  These tests have largely consisted of executing queries that should make it into the transaction log, then using the UDF print_transaction_message($log_file,$log_offset) to examine the log's contents.  The tests can be found <a href="https://code.launchpad.net/~patrick-crews/drizzle/transaction_log_tests">here</a> and executed with ./test-run --suite=transaction_log.  (NOTE:  The tests themselves are largely complete, but our expected results are not yet finalized / correct due to the bugs noted below).  I'd like to extend a special thanks to Joe Daly for his help in writing these tests and finding some bugs in the log.</div></br></br>


<div id="_mcePaste">While we have tested all of the available data types and basic transactions and they are looking quite solid, our efforts have still turned up some interesting bugs:</div>
<div id="_mcePaste">(this list is maintained at the launchpad blueprint noted above)</div></br>
<div id="_mcePaste">
<ul>
	<li>Bug #594873: transaction log incorrectly records NULL INSERT into an ENUM as the first permissible value</li>
	<li>Bug #594876: transaction log not differentiating NULL values and empty string for char columns</li>
	<li>Bug #596972: transaction log logging 0 for NULL INTEGER VALUES</li>
	<li>Bug #599582: Transaction log does not appear to be collecting all information for multi-row REPLACE statements</li>
	<li>Bug #597910: Transaction log does not appear to be capturing FOREIGN KEY information</li>
	<li>Bug #599851: Transaction log not capturing CASCADE'd UPDATE data on a table using a foreign key</li>
	<li>Bug #599952: transaction log attributing statements to wrong tables on multi-table, multi-statement transactions</li>
	<li>Bug #600032: rollback to savepoint not handled correctly in transaction log</li>
	<li>Bug #600795: LOAD DATA INFILE INSERTs not registered by the transaction log</li>
</ul>
</div></br></br>
<div id="_mcePaste">The first 3 bugs relate to how the log captures NULL values for various data types and have been traced to a single root cause.  The remaining 6 seem more interesting and serious for replication functionality.  To summarize, the transaction log appears to have trouble with trickier (more complex) transactions.  These include changes propagated via a foreign key, multi-row REPLACE, and multi-table transactions.</div></br></br>
<div></div>
<div></div>
<div id="_mcePaste">Once these bugs have been addressed, we will continue with test development for the randgen.  This will include stress testing the server / log with DDL-generating grammars and validation of the data stored within the log.  Initial experiments with high-volume (10+ threads at 250k queries each) have looked promising (no crashes, locks, major slow downs over time).  In the meantime, we'll be busy with <a href="https://blueprints.launchpad.net/drizzle/+spec/test-dump-restore">other tasks</a> (dump+restore)</div></br></br>
<div></div>
<div id="_mcePaste">As always, we welcome any feedback, questions, or bug fixes : )</div>
<div id="_mcePaste">More information on Drizzle testing can be found <a href="http://drizzle.org/wiki/DrizzleQA">here</a>.</div>
