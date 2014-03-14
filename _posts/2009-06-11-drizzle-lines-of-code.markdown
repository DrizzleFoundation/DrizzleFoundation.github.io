---
layout: post
status: publish
published: true
title: Drizzle lines of code
author: Lee Bieber
author_login: lbieber
author_email: kalebral@gmail.com
wordpress_id: 90
wordpress_url: http://blog.drizzle.org/?p=90
date: 2009-06-11 07:50:30.000000000 +00:00
categories:
- This Week In Drizzle
tags: []
comments: []
---
Jay along with help from many of you has done a great job automating a lot of our tools to provide Drizzle metrics to get a handle on how we are doing. You've seen the regular emails that now generate <a href="https://launchpad.net/sysbench">sysbench</a> numbers for each build, we also have regular automated builds to generate data for <a href="http://valgrind.org/">valgrind</a>, <a href="http://drizzle.org/lcov/">lcov</a>, <a href="http://drizzle.org/doxygen/">doxygen</a> and <a href="http://www.dwheeler.com/sloccount/">sloc</a>. Oh and lets not forget <a href="http://gorf.tangent.org/source/">OpenGrok</a> which was setup by Trond.

If you look at lcov we still have a few rough edges to work out and actually could use some help if any of you are familiar with the inner workings of lcov. 

The sloc graph below is showing data going back to March. Nice steady progress downwards which in this case is great! The big drop around build 960 was due to plugin clean up work by Monty and the slight increase around build 984 was from protocol work from Eric (all necessary and important!). Now if we could get one of you to help generate a nice dynamic web page to display this information......any takers?

<img src="http://173.203.216.19/wordpress/wp-content/uploads/2009/06/drizzle-lines-of-code-300x224.jpg" alt="drizzle-lines-of-code" title="drizzle-lines-of-code" width="600" height="374" class="alignnone size-medium wp-image-105" />
See <a href="http://drizzle.org/wiki/Image:Drizzle_Lines_of_Code.pdf">here</a> for a pdf of the graph
