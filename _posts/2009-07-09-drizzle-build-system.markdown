---
layout: post
status: publish
published: true
title: Drizzle Build System
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 156
wordpress_url: http://blog.drizzle.org/?p=156
date: 2009-07-09 19:34:09.000000000 +00:00
categories:
- This Week In Drizzle
tags: []
comments: []
---
I wanted to follow up from <a href="http://krow.livejournal.com/638654.html">Brian's blog</a> last month where he was talking about how we do our testing in the <a href="http://launchpad.net/drizzle">Drizzle</a> project. Brian mentioned our build system and I thought I would expand on that. 

Right now in Drizzle we use both <a href="https://hudson.dev.java.net/">Hudson</a> and <a href="http://buildbot.net/trac">Buildbot</a> for automated and continuous builds. Our dashboards can be seen <a href="http://solace.inaugust.com/">here</a> and <a href="http://gorf.tangent.org/hudson/drizzle/">here</a>.  We use both email and IRC for notifications when builds fail. While the dashboards are not as Green as we would like right now, we are only a few fixes away from having it generally back on track and our goal is to keep it on track as we move forward! 

We have a wide variety of build clients as you can see and run our build process from both the trunk and staging code base. All changes first go through staging for verification which means making sure it still builds (warnings are always treated as errors), passes all unit tests (no disabling of tests) and has not regressed in our <a href="http://drizzle.org/performance/">sysbench numbers</a>.  After code is promoted to trunk we also run updates for <a href="http://drizzle.org/lcov/">LCOV</a>, <a href="http://drizzle.org/sloc/">SLOC</a> and <a href="http://drizzle.org/doxygen/">Doxygen</a>.  Trond</a> also set up regular runs for <a href="http://gorf.tangent.org/source/">OpenGrok</a>. 

Jay</a> put together a great <a href="http://drizzle.org/wiki/Automation_Documentation">automation system</a> to run sysbench, doxygen, lcov, sloc as well as the ability to run  Valgrind tools as part of the sysbench run. Eric and Monty also extended this to use <a href="http://www.gearman.org/">Gearman</a> so we can <a href="http://drizzle.org/wiki/Gearman_Integration">submit jobs</a> on demand to various machines if we want to run jobs out of cycle. 

Thanks to <a href="http://michaelshadle.com/">Michael Shadle</a> for putting together our <a href="http://drizzle.org/performance/">fancy graphs</a> on the wiki and also donating a few machines for buildbot clients. 

Always looking for more clients so if you have a machine you can provide, let us know.  

Any suggestions for improvement? 
