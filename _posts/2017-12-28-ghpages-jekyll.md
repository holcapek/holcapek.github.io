---
title: GitHub Pages & Jekyll
layout: post
---
### Install Jekyll & GitHub Pages requirements

{% highlight bash %}
$ sudo dnf install ruby ruby-devel rubygem-bundler
{% endhighlight %}

### Install [GitHub Pages gem](https://jekyllrb.com/docs/github-pages/#the-github-pages-gem)

{% highlight bash %}
$ cat > Gemfile
source 'https://rubygems.org'
gem 'github-pages'
gem 'json'
{% endhighlight %}

{% highlight bash %}
$ bundle install
{% endhighlight %}

### Configure Jekyll

This is pretty minimalisic configuration. For more, see Jekyll [Configuration](https://jekyllrb.com/docs/configuration/).

{% highlight bash %}
$ cat > _config.yml
markdown: kramdown
markdown_ext: md
highlighter: rouge
{% endhighlight %}

### Run Jekyll locally

{% highlight bash %}
$ jekyll serve -w -D
{% endhighlight %}
