---
layout: post
title:  "Create your Jekyll Blog on GitHub Pages"
date:   2017-10-23 15:00:00 +0200
categories: jekyll github
---
Hi, I guess you are here to create your own [Jekyll][jekyll-website]  website on GitHub Pages.

Easy, peasy, cheesy.

First, you need a GitHub account.
... Your website will be hosted by GitHub Pages, based on your repository.

Second, install Jekyll locally.
... here are the shell commands on Ubuntu :
{% highlight shell %}
# first install Ruby
apt-get install ruby-full
# then install jekyll
gem install jekyll bundler
# then create your jekyll blog
jekyll new myblog; cd blog;
# ....
{% endhighlight %}

Third, get a decent badass theme.
... There are plenty of jekyll theme you can try.
I suggest you to try the jekyll minimal theme first to get your hands on.

Fourth, I assume you already know how to Git...
...
if not U_NO_HOW_2_GIT:
    go_learn_git()

-Create a repository with that name '[your_github_account].github.io'
Make sure it's host here : https://github.com/[your_github_account]/[your_github_account].github.io.

Fifth, on your local env:
{% highlight shell %}
# do some shell commands to create a jekyll blog with the chosen theme
# I chose https://github.com/yous/whiteglass
{% endhighlight %}

-Make some modifications : Go ahead and edit it and re-build the site to see your changes.

-Run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.
If you don't want several terminal opened :
`jekyll serve --detach` with do the same but the process will be detach from your terminal.
No worries, if you need to kill it, jekyll will tell you :
{% highlight shell %}
#    If you need to kill the server, you can `kill -9 1234` where "1234" is the PID.
#    If you cannot find the PID, then do, `ps aux | grep jekyll` and kill the instance.
{% endhighlight %}

-When you statisfied of your website,
commit and push your modifications on that repository of yours '[your_github_account].github.io'

-Github Pages will deal the rest now.
Remember, it has jekyll builtin, and for every commit, Github will generate your jekyll base website.
So you can check your new website at http://[your_github_account].github.io'/

You learned to setup jekyll and your static website on github page.
That's it !

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll.

[jekyll-website]: https://jekyllrb.com/
[jekyll-docs]: https://jekyllrb.com/docs/home
