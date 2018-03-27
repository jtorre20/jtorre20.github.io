---
layout: post
title:  "Managing Our Remote Repositories"
date:   2018-03-28 21:35:18 -0400
categories: Git Basics
---
<!--You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.-->
<!---->
<!--To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.-->
<!---->
<!--Jekyll also offers powerful support for code snippets:-->
<!---->
<!--{% highlight ruby %}-->
<!--def print_hi(name)-->
<!--  puts "Hi, #{name}"-->
<!--end-->
<!--print_hi('Tom')-->
<!--#=> prints 'Hi, Tom' to STDOUT.-->
<!--{% endhighlight %}-->
<!---->
<!--Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].-->
<!---->
<!--[jekyll-docs]: https://jekyllrb.com/docs/home-->
<!--[jekyll-gh]:   https://github.com/jekyll/jekyll-->
<!--[jekyll-talk]: https://talk.jekyllrb.com/-->

Managing remote repositories can include adding remote repositories, removing remotes that are no longer valid, managing various remote branches and defining them as being tracked or not among an array of many other valuable skills.

What doe "Remote" even mean?

Lets decode and clear up what it means for something to be remote. If we break it down to its simplest explanation,
to be remote is just to be elsewhere. It is within reason to think of something that is remote as existing somewhere else on the network/Internet.  However, this doesn't always have to be the case. We could be working on a remote branch that resides on our host machine.

Git Commands

In order to see a list of the remote servers that we have configured we use {% highlight %} git remote {% endhighlight %}. The server which you clone from is labeled and known as {% highlight %} origin {% endhighlight %}. Personally, I find this nomenclature easier for remembering out which is the original branch. 
