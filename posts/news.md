---
layout: for_include
title: OSHChip V1.0
excerpt: "Product Description"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-01-26
image:
  feature: header.jpg
---

This is all dummy stuff to get the HTML fragment that we MANUALLY
copy to /_include/news.html

All the solutions I found to expand xxx.md within an HTML file
(such as home_no_recents.html) won't work with Jekyll on GitHub
because it doesn't support plugins.

VERY VERY VERY VERY VERY VERY  crapy solution, but it is time to move on

Here are the steps:

1) edit this file /posts/news.md
2) on save, jekyll will create an html here: /_site/posts/news.html
3) open /_site/posts/news.html  and select&copy the HTML fragment we wanted
4) paste it into /_include/news.html
5) in the html file that we wanted to include news.md , place
	include news.html
	surrounded by curly brace and percent.


###News

* **Monthly News Letter** <a href="http://goo.gl/forms/K2Qlvjiobx" target="_blank">Newsletter Signup</a>
* The web site now has a Forum
* OSHChip is considering making the unique custom pins available as a product. Please send an email to the above link to help with estimating production size.
