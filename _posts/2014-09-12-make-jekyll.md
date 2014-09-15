---
layout: post
title:  "Make Jekyll"
---
- [How to setup Jekyll Blog Hosted on GitHub Project Pages](http://openjerseycity.org/blog/technical/2014/06/18/Jekyll-On-GitHub-Pages/)

ruby version was 2.0.0-p481
add Gemfile `gem 'github-pages'`

{% highlight bash %}
~ $ bundle install
~ $ jekyll new my_blog
~ $ cd my_blog
{% endhighlight %}

add a new repository on Github called `my_blog`

{% highlight bash %}
~/my_blog $ git init
~/my_blog $ git checkout -b gh-pages
{% endhighlight %}

edit `_config.yml` with url and baseurl 

{% highlight yaml %}
baseurl: "/my_blog"
url: "http://kangkyu.com"
{% endhighlight %}

push it to Github and I checked url `http://kangkyu.com/my_blog`

{% highlight bash %}
~/my_blog $ git add .
~/my_blog $ git commit -m "a comment"
~/my_blog $ git push origin gh-pages
{% endhighlight %}

add files under `_posts` directory and edit while checking preview as needed.

- [Highlighting Code Snippets](http://jekyllrb.com/docs/posts/#highlighting-code-snippets)
- [Front Matter](http://jekyllrb.com/docs/frontmatter/)
- [Jekyll Documentation](http://jekyllrb.com/)
- [Jekyll on Github Pages](https://help.github.com/articles/using-jekyll-with-pages#installing-jekyll)

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help