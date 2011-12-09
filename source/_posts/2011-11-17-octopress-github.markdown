---
layout: post
title: "Octopress - Github"
date: 2011-11-17 00:27
comments: false
categories:
---

This post describes how to setup a [github][001] account and repository that [Octopress][002] will use. Github will store your data and host your blog (for free).

<!--more-->

## Assumptions

* You are using Linux
* You do not have an existing github account.
* After creating an Account you stay logged into github.

## Step: Create Account
Go [here][003]. The image below shows creating an account for user1999 with email youremail@gmail.com.

{% img /images/001.png %}

## Step: Configure Account
Go [here][004]. Follow the instructions under the 3 main subheadings.

* First: Download and Install Git
* Next: Set Up SSH Keys
* Then: Set Up Your Info

## Step: Create Repository
Go [here][005]. The important thing you need to do here is in the **project name field** enter **username.github.com**, where username is the name you used to setup your github account. The image below shows creating a repository for user1999.

{% img /images/002.png %}

## Step: Fini
To find how to install Octopress to use this new repository go [here][006]

[001]: http://github.com
[002]: http://octopress.org
[003]: https://github.com/signup/free
[004]: http://help.github.com/linux-set-up-git/
[005]: https://github.com/repositories/new
[006]: http://heterodoxic.com/blog/2011/11/18/octopress-installation/

