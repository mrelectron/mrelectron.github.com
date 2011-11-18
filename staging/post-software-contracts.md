---
layout: post
title: "Automating Software Contracts"
date: 2011-11-16 00:27
comments: true
categories:
---
## NOTES
* the microsoft dotnet way - seems to work, os dependent
* contract + uri - my way. what does a contract look like, how do we enforce it?
* dpkg way - central repository - works ok, os dependent

## Introduction
This article is really aimed at FOSS projects, maybe we are spending a lot of time writing documentation that does not get read, gets out date quickly and generally is useless and does more harm than good to our reputation. A user may want to use the software has problems with the installation cannot resolve them and gives up.

This post will describe how to install [Octopress][] on [Ubuntu Oneiric][]. There are many other guides to installation out there, see the references for those other guides. In this post I will experiment with using [topic based help][]. I read [somewhere][], that guided instruction is not really that helpful. The way that people use technical help is not to use it until they get stuck then they want just the little bit of focused help to get them over that immediate hurdle then they will go on with the task until they hit another hurdle. This struck with me, becauses that is how I use help.

The process I go through when I start a technical task such as installing and configuring a piece of software is

* Been motivated to do the task through reading some article or blog post. Thats my 30,000 foot view.

* I may do some further research which will involve Google to find out what other people think.

* Then I will use the software documentation itself to guide me through the installation process.

* When that guide fails as it invariably does for non-trivial installations. I will just make the point here that most software I use is [FOSS][] based written in various languages and running on Linux variants, where the documentation component of the project invariably has suffered in comparison to the programming component. That's actually OK, I would rather have bug free software with poor documentation than buggy software with great documentation. Which raises the issue of that it may be worthwhile for developers to spend a certain of time on a foolproof automated installation for their software or someone to devise a generic linux based installation tool (that sounds hard).

* I digress so I'm upto the point where I have read and followed the software installation documentation, at some point their is a failure and the documentation does not give any indication of how to troubleshoot the problem. Now I need to do further Googling to find out how to solve the problem. Which will generally involve Google for the particular error, find someone who has done the installation themselves, raise the issue with the developers. My assumption here is that raising the issue with the developers is not appropriate because it will be too slow or they are too busy and I should try harder to solve it myself. So I will usually just apply the first two heuristics.

* So now I'm at the point where I'm following a fairly standard problem solving routine. Which algorithm is really just: while no solution found: keep googling for a solution. Really kind of imperfect.

* If we step back to our starting point, the actual problem is that software documentation for the installation process was not sufficient, there could be many reasons for this, for example related to versions, or related to dependent library versions of operating system versions. Oops there is a pattern emerging here. Most problems seem to arise when then there is differing versions of the various software components in play or new dependencies on other libraries emerge. So the software has been written and tested on a particular platform or platforms, but not all platforms and variants as there are so many. Also subsequent iterations of the software will quickly get out of sync if the documentation is not kept upto date.

* Assuming we cannot fix the version / dependency problem which is a monster problem. How can we ameloriate the problem for the user. We must have to offer help that is not dependent on any particular version of the software. But all software has these dependencies and if it is not smart enough to work out what they are itself then we must empower the user to do something to get the correct components. This is also a very hard problem, so we have to lower our sights.

* I'm painted into a corner here. The resolution of this problem must come from upstream. The developer must produce self installable software that is smart enough to know its environment work out what it needs to run, get it, integrate it and install itself.

* This problem is sometimes found on Windows but it is not a big problem because services provided by the OS to individual applications are written by a single organisation. Other services will be written by the application developers themselves and included with the application.  The Linux / FOSS problem is that supporting services used by the application are written hetergenous group of people who in most cases have no connection with the application in question and who different objectives and priorities and who are pushing out new versions of the library or service which are then included in various operating system distributions. At this point software installations start to fail.

* Maybe when an application developer starts to use services from another library. Some type of formal contract needs to be involved formal in the sense of an automated agreement. This would need to start from the top. So for example Ubuntu Oneiric would have thousands of these automated agreements if not tens of thousands or hundreds of thousands of these agreements. Something like this must already exist in the Ubuntu packaging system. So we need a application packaging system that is language agnostic all it cares it needs x,y,z components with this particular build and version and found at this particular uri.

* So lets look at an example. This post started with me going to document an Octopress installation, which is advertised as a hackers blog. I cannot say the installation went smoothly, the Octopress part did but it has a dependency of Ruby 1.9.2 so thats where everything fell apart. I had to compile Ruby 1.9.2 for Ubuntu 11.04, and then I upgraded to Oneiric which was still running Ruby 1.8.7, the same compilation process that worked on 11.04 did not work on 11.10. Long story short, got Ruby 1.9.2 working on 11.10. Octopress installation went sort of smoothly apart from some problems with bundle.

* what would have worked for me was to type in Octopress --install. it reads it service contract, checks the environment, gets what it needs builds itself and I can use it. That would be so great would it not. So when the service contract said it needs Ruby 1.9.2 it would have got Ruby 1.9.2 from its uri, read the Ruby 1.9.2 contract got any relevant librarys or services required by Ruby built Ruby, then built itself.

* Anyway I'm still digressing I should get back to the original task. I will investigate this contract proposal see what is out there.
