---
layout: post
status: publish
published: true
title: Drizzle.org was unavailable today, domain now successfully transferred to SPI
author: Patrick Crews
author_login: pcrews
author_email: gleebix@gmail.com
wordpress_id: 1193
wordpress_url: http://blog.drizzle.org/?p=1193
date: 2011-11-08 14:37:00.000000000 +00:00
categories:
- Uncategorized
tags: []
comments:
- id: 211
  author: Elisamuel Resto
  author_email: sam@simplysam.us
  author_url: http://simplysam.us
  date: '2012-01-06 08:35:13 +0000'
  date_gmt: '2012-01-06 16:35:13 +0000'
  content: '... and like many sites on the internet, www.drizzle.org works but not
    drizzle.org (because the latter has no A records).'
---
The entire <a href="http://www.drizzle.org/">drizzle.or</a>g domain was unavailable for about 10 hours today. This made our website, documentation, jenkins master and mail server inaccessible. On the other hand as we use public services such as Launchpad and Freenode for code repository, bug tracking, mailing list and IRC, this meant that development work continued as active as ever - in fact I think it was the most active day on IRC #drizzle channel in a while!

The DNS outage was related to our transferring of the drizzle.org domain from an individual Drizzle developer to <a href="http://blog.drizzle.org/2011/10/06/drizzle-is-now-member-of-software-in-the-public-interest-can-take-donations/">Software in the Public Interest, Inc</a>, our umbrella non-profit corporation. We don't know exactly why, but something went wrong between the registrars, so that the Whois record listed Tucows, the sponsoring registrar used by SPI, as the new registrar, but all other information was still pointing to the old registrar, including some Godaddy nameservers. As Godaddy eventually stopped answering DNS queries for drizzle.org - as they should - the drizzle.org domain became unavailable. 10 hours later the issue was fixed, and the correct SPI nameservers started to propagate through the DNS system. At the time of this writing, everything should have been working normally for some hours already.

And yes, in related news, drizzle.org is now transfered to the ownership of <a href="http://spi-inc.org/">Software in the Public Interest</a>. This is yet another step in our process of becoming a solid non-profit community project, with fiscal services provided by the SPI. So far the experience has been enjoyable and we've really felt a warm welcome into the family of SPI hosted free and open source software projects.

On that note I'd like to thank Ganneff, Solver, Hydroxide and weasel from the #spi  channel for actively helping in troubleshooting and fixing the problem today.
