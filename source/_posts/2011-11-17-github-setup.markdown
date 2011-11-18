---
layout: post
title: "Github - Hosting for Octopress"
date: 2011-11-16 00:27
comments: false
categories:
---

## Introduction
This post describes how to setup a [github][001] account and repository that [Octopress][002]can use. Github will store your data and host your blog (for free). Some assumptions have been made in this post, firstly you are using Ubuntu and secondly you do not have an existing github account.

## Create github account
Go [here][003].

{% img /images/001.png %}

{% blockquote %}
You need to be logged into github to complete the following two steps.
{% endblockquote %}

## Configure github account
Go [here][004]. Follow the instructions under the 3 main subheadings.
* First: Download and Install Git
* Next: Set Up SSH Keys
* Then: Set Up Your Info

## Create a github repository
Go [here][005]. The important thing you need to do here is in the project name field enter username.github.com, where username is the name you used to setup your github account above.

{% img /images/002.png %}

## Fini
We are finished setting up github and can now start on setting up Octopress, this will be another post.

[001]: http://github.com
[002]: http://octopress.org
[003]: https://github.com/signup/free
[004]: http://help.github.com/linux-set-up-git/
[005]: https://github.com/repositories/new
