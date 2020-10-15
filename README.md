# README

* Ruby version
2.6.5

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Alchemy setup:
# add 'alchemy_cms' into Gemfile with git URL
# bundle update
# bundle add alchemy-devise
# rake alchemy:install
# visit localhost:3000 after rails s

Alchemy first use after git clone:
# rails db:migrate
# rails db:seed
# rails s
# goto localhost:3000 to setup your first user

To add new page layout for you to choose when creating pages:
# go to config/alchemy/page_layouts.yml
# Follow https://guides.alchemy-cms.com/pages.html#defining-page-layouts and add new layout template
# update config/alchemy/elements.yml too


KNOWN ISSUES
# 'rails g alchemy:page_layouts --skip' does not work
