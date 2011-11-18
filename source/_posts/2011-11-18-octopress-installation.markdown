---
layout: post
title: "Octopress - Installation"
date: 2011-11-18 11:13
comments: true
categories:
---

This post describes the process to install [Octopress][001] on [Ubuntu Oneiric 11.10][002]. My starting point was a brand spanking new install of Oneiric on a [Virtual Box][003] virtual machine. Immediately after this installation completed I did a sudo apt-get -y update && sudo apt-get -y upgrade.


<!--more-->

## Assumptions

* You are not logged in as root.
* Git is installed on your computer. If not a simple sudo apt-get -y install git will suffice.
* You have created your github account and Octopress repository, if you have not go [here][007].

## Step: Get Ruby
Oneiric comes with Ruby 1.8.7. Octopress depends on Ruby 1.9.2.

{% codeblock %}
& sudo apt-get -y install ruby1.9.1-full
& sudo update-alternatives --set ruby /usr/bin/ruby1.9.1
& sudo env REALLY_GEM_UPDATE_SYSTEM=1 gem update --system
{% endcodeblock %}

## Step: Test Ruby
The important thing is the Ruby version is at least 1.9.2.

{% codeblock %}
& ruby -v.
& ruby 1.9.2p290 (2011-07-09 revision 32553) [i686-linux]
& gem -v
& 1.8.11
{% endcodeblock %}

## Step: Get Octopress
{% codeblock %}
& mkdir ~/name_and_location_you_choose
& cd ~/name_and_location_you_choose
& git clone git://github.com/imathis/octopress.git octopress
{% endcodeblock %}

## Step: Configure Octopress
{% codeblock %}
& cd octopress
& sudo gem install bundler
& bundle install
& rake install
& rake setup_github_pages
Enter the read/write url for your repository: git@github.com:uname/uname.github.com.git
{% endcodeblock %}

## Step: Generate & Deploy
{% codeblock %}
& rake generate
& rake deploy
{% endcodeblock %}

## Step: Commit Source
{% codeblock %}
& git add .
& git commit -m 'Initial Commit'
& git push origin source
{% endcodeblock %}

## Step: Fini
All finished, you can blog. Go [here][009] for some simple instructions on how to write your first post. Go [here][008] for some simple instructions on making minor modifications to the look of your blog, such things as changing the name of the blog, the name of the author and enabling various services such as Disqus, Twitter etc.


## References

* [Gregory A. Lussier][004]
* [Victor Costan][005]
* [Adriene Lamothe][006]

[001]: http://octopress.org
[002]: http://www.ubuntu.com/
[003]: https://www.virtualbox.org/
[004]: http://greglus.com/blog/2011/10/10/how-to-install-octopress-on-ubuntu/
[005]: http://blog.costan.us/2011/10/getting-mri-192-on-ubuntu-1110.html
[006]: http://answers.oreilly.com/topic/2845-installing-ruby-1-9-on-a-debian-or-ubuntu-system/
[007]: http://heterodoxic.com/blog/2011/11/16/github-setup.html
[008]: http://octopress.org/docs/configuring/
