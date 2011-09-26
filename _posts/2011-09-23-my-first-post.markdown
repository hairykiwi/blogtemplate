---
layout: post
title: Hosting your blog with GitHub pages
---

Okay, [GitHub Pages](http://pages.github.com/) is pretty amazing. [Jekyll](https://github.com/mojombo/jekyll/wiki) just makes it even more magic, as it will apply templates to your posts giving you plenty of control over formatting, but allowing you to easily change your site.

The beauty of hosting a blog this way, is the pages are completely static. So delivery time is always going to be incredibly quick. Running Wordpress using a shared server instance, I was getting around 1000msec to deliver an incredibly light homepage. On GitHub, that's normally down around the 150-180msec range. Pretty much an order of magnitude faster.

And these days, speed counts. Especially if your blog gets slashdotted/reddited/digged (well, maybe not digg any more) or HackerNews'd. The static site has a good chance of surviving that load. Admittedly, a well cached Wordpress site should do as well, but I've lost count of the number of unavailable Wordpress blogs when the going gets tough.

And that's not to say your site has to be completely static either. You've always got things like Disqus/Facebook or GetSatisfaction to dynamically include commenting on your site without adding extra load to your server.