PictureFace
========================

The purpose of this Project is to build an Instagram clone

* I started the project by using the rails command `rails new picture_face -d postgresql -T` in order to intialize the project using PostgreSQL as my database and without the default testing framework

* The next step was to set up development and testing databases like so
```
bin/rake db:create
bin/rake db:migrate
bin/rake db:create RAILS_ENV=test
bin/rake db:migrate RAILS_ENV=test
```
* I set up the Rspec as my testing framework by adding the following to my Gemfile and running `bundle`
```
group :test do
  gem 'rspec-rails'
  gem 'capybara'
end
```
* I then ran `bin/rails generate rspec:install` in order to get rspec going by creating a spec directory with 2 helper files, spec/spec_helper.rb' and 'spec/rails_helper.rb, and a .rspec behaviour configuration file

* In order to allow capybara testing I added the line `require 'capybara/rails'` to spec/rails_helper.rb

Instagram Challenge
===================

Instructions
-------
* Challenge time: Friday, the entire day + the weekend if you need it
* Feel free to use Google, your notes, books, etc., but work on your own
* If you refer to the solution of another coach or student, please put a link to that in your README
* If you have a partial solution, **still check in a partial solution**
* You must submit a pull request to this repo with your code by 9am Monday morning

Task
-----

Build Instagram: Simple huh!

Bonus if you can write your own set of sensible user stories!

As usual please start by forking this repo. After cloning your fork and cd'ing into it, you'll need to [initialize a Rails app in the current directory](http://blog.jasonmeridth.com/posts/create-rails-application-in-current-directory/).

Your challenge is to build Instagram using Rails. You'll need **users** who can post **pictures**, write **comments** on pictures and **like** a picture. Style it like Instagram's website (or more awesome).

Bonus if you can add filters!
