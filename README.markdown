# Demo application for Ruby and Rails installation

[* A simple demo application*](sujith.com)
by [Sujith](sujith.com)
== Welcome to Rails

https://github.com/gmate/gmate
install curl        sudo apt-get install curl

RVM INSTALLATION = 

REQUISITES=     * * * Very very important
/usr/bin/apt-get install build-essential openssl libreadline6 libreadline6-dev curl git-core zlib1g zlib1g-dev libssl-dev libyaml-dev libsqlite3-0 libsqlite3-dev sqlite3 libxml2-dev libxslt-dev autoconf libc6-dev ncurses-dev automake libtool bison subversion

https://rvm.beginrescueend.com/rvm/basics/

CHANGE .profile accordingly .profile or .bash_profile
echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm" # Load RVM function' >> ~/.profile


rvm list known

rvm install ruby-1.9.2-p290
rvm install ruby-1.9.3-p0

rvm use 1.9.2
rvm use 1.9.3

ruby -v

which ruby


rvm use 1.9.2 --default
rvm use 1.9.3 --default

type rvm | head -1
does not  show "rvm is a function", RVM isn't being sourced correctly.


https://rvm.beginrescueend.com/rvm/basics/


= ================================ =

INSTALLING RUBY GEMS
http://rubygems.org/pages/download
Extract the download
  ruby setup.rb 


rvm use 1.9.3 --default
gem install rails


gmate Gemfile
  gem 'execjs'
  gem 'therubyracer'

bundle




##############################
ERRORS =============

gem install rails
ERROR:  Loading command: install (LoadError)
    cannot load such file -- zlib
ERROR:  While executing gem ... (NameError)
    uninitialized constant Gem::Commands::InstallCommand
------------------------
SOLUTION
Remove the problem making lib reinstall ruby

    rvm pkg install zlib

    rvm remove 1.9.3

    rvm install ruby-1.9.3-p0

= ======================================================================================== =
        GIT
= ======================================================================================== =
git init



= ======================================================================================== =
HEROKU
= ======================================================================================== =

http://api.heroku.com/signup
gem install heroku
heroku keys:add
heroku create
git push heroku master
heroku open
heroku rename sujith-demo




















