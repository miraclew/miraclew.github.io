---
layout:     post
title:      "Github pages and Jekyll"
subtitle:   "How to use Jekyll to setup a blog and host on Github pages"
date:       2014-11-23 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>Install Ruby & Jekyll</h2>

Install rvm and ruby:
 * `\curl -sSL https://get.rvm.io | bash -s stable`
 * `source /home/bob/.rvm/scripts/rvm`
 * `rvm install ruby-2.1`
 * `gem install jekyll`

<h2>Choose a template</h2>
<p>
	Search on the web to find your favorite theme.
	For example, my blog theme is Clean Blog by Start Bootstrap - Jekyll Version.
	https://github.com/IronSummitMedia/startbootstrap-clean-blog-jekyll
</p>

<h2>Run blog on local</h2>
`jekyll serve --watch`

open browser and navigate to http://localhost:4000/

<h2>Push to github</h2>
<p>
	After you finished composing your blog, push it to github, and check it out on github.io,
	like http://miraclew.github.io
</p>

