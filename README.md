# README

* Ruby version
    * 2.6.5
* System dependencies
    * rails 6.0.3
    * sqlite3


## Alchemy setup:
* make sure you install rails 6
* rails new alchemy_cms_example
* cd alchemy_cms_example
* rm Gemfile.lock
* Add the following to Gemfile
	* `gem 'alchemy_cms', :git => 'git://github.com/AlchemyCMS/alchemy_cms', :branch => '5.0-stable'`
    * `gem "alchemy-devise", github: "AlchemyCMS/alchemy-devise", branch: "master"`
* bundle install
* rake alchemy:install
* rails g alchemy:devise:install
* visit localhost:3000 after rails s

## Alchemy first use after git clone:
* rails db:migrate
* rails db:seed #(optional)
* rails s
* goto localhost:3000 to setup your first user

### Use after created first user
* goto localhost:3000/admin/login
* type in your username & password
* you should able to access the dashboard

### To add new page layout for you to choose when creating pages:
* go to config/alchemy/page_layouts.yml
* Follow https://guides.alchemy-cms.com/pages.html#defining-page-layouts and add new layout template
* update config/alchemy/elements.yml too

## KNOWN ISSUES
* 'rails g alchemy:page_layouts --skip' does not work (resolved by alchemy-devise master branch)
