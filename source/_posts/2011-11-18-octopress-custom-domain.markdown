---
layout: post
title: "Octopress - Custom Domain"
date: 2011-11-18 17:10
comments: true
categories:
---

This post describes the process whereby you can use your own domain name to point to your blog. Useful background information can be found [here][001]. Look under subheadings "User & Organization Pages" & "Custom Domains"

As an example of what we are going to do, my github username is mrelectron, I have a repository accessible at the internet address http://mrelectron.github.com. But I want to access this repository using a domain name that I own called heterodoxic.com

## Assumptions

* You have a working Octopress installation.
* You own a domain name
* You have edit / add permission for your domain name DNS records.

## Step: Create CNAME file
Using the editor of your choice create a file called CNAME in the source directory of your Octopress installation. On the first line put the domain name that you want to point to your Octopress installation.

{% img /images/004.png %}

## Step: Commit CNAME file
Committing this file to the repository will signal to the github server it needs to map requests for heterodoxic.com to mrelectron.github.com
{% codeblock %}
& git add .
& git commit -m 'Adding CNAME file'
& git push origin source
{% endcodeblock %}


## Step: Modify DNS Records
I cannot be specific here as DNS management user interfaces are going to vary wildly. I added a single "A" DNS record that points at 207.97.227.245 which is github.com. The @ in the image is shorthand for heterodoxic.com.

{% img /images/005.png %}

## Step: Fini
All done, it may take some time for the change made to your DNS, to propagate around the world. If it does not work after 24 hours though, you may have a problem.

# References
[001]: http://pages.github.com/

