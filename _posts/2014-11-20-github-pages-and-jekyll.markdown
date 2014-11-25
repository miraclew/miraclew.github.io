---
layout:     post
title:      "Github pages and Jekyll"
subtitle:   "How to use Jekyll to setup a blog and host on Github pages"
date:       2014-11-23 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>Install Ruby & Jekyll</h2>

Install rvm:

 `$\curl -sSL https://get.rvm.io | bash -s stable`

 `$source /home/bob/.rvm/scripts/rvm`

Install Ruby

 `$rvm install ruby-2.1`
 
Install jekyll

 `$gem install jekyll`

<h2>Choose a template</h2>
<p>
	Search on the web to find your favorite theme.
	For example, my blog theme is
	<a href="https://github.com/IronSummitMedia/startbootstrap-clean-blog-jekyll">Clean Blog by Start Bootstrap - Jekyll Version</a>
</p>

<h2>Run blog on local</h2>
Run the command on the root directory on your blog

`jekyll serve --watch`

open browser and navigate to http://localhost:4000/

<h2>Push to github</h2>
<p>
	After you finished composing your blog, push it to github, and check it out on github.io,
	like <a href="http://miraclew.github.io">http://miraclew.github.io</a> 
</p>

