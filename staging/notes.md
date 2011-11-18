## Octopress - Custom Domain
custom DOMAIN. with github.
add CNAME file with tld to source dir. then do the dns stuff at your provider.

## Understanding
1. website contents located in master branch.
2. application source in source branch.
3. create post: rake new_post["title"].
4. located in source/_posts.
5. rake generate & rake deploy to update website & contents.
6. rake will generate from source folder and deploy to _public folder.
7. always "git push origin source" to update your Github Repository
octopress root is the working directory.
_deploy is the local repository
origin is the remote master repository on mrelectron.github.com/master to which we push up changes from our local repo
we end up with two branches master & source why is that.
    master is the webroot
    source is octopress root + source directory.

## Environment
* virtual box - virtual machine
* Ruby 1.9.2
* Not using RVM
* Ubuntu 11.10 Oneiric
* Octopress 2.0
* Github Backend

## Troubleshooting
bundle install and permissions on ~/.gem use sudo  bundle install
The program 'rake' is currently not installed.  You can install it by typing:
sudo apt-get install rake NO DONT DO THIS. for some reason the bundle install did not put the gem binaries into /usr/bin, when i reran it by removing gemfile.lock and bundle install it worked.
sudo gem install places gem into system gem location
gem install places gems into user gem location eg ~/.gem
problems in this area (1) not putting binaries on path (2) not installing gems to ~/.gem
using wrong readwrite url.
cache not empty so was geting old pages.
git add . / git commit seem to have to use them together.
openssl error on ruby compile
no ruby-bundle package
incorrect ruby version
bundles puts gems in system gems not ~/.gems
