# Cucumber-Rails2.3.x

Cucumber-Rails2.3.x brings Cucumber to Rails 2.3.x. For Rails 3.x support, see the [README](https://github.com/cucumber/cucumber-rails/blob/master/README.md) 

It contains 2 generators - one for bootstrapping your Rails app for Cucumber, and a second one for generating features.

Cucumber-Rails also contains Cucumber Step Definitions that wrap Capybara or Webrat,
giving you a head start for writing Cucumber features against your Rails app.

## Installation

### Rails 2.3.x:

Before you can use the generator, install the gem by running:

  gem install cucumber-rails

Learn about the various options:

  ruby script/generate cucumber --help

Finally, bootstrap your Rails app, for example:

  ruby script/generate cucumber --rspec --capybara

## Generating a Cucumber feature

IMPORTANT: Only do this if you are new to Cucumber. We recommend you write your
Cucumber features by hand once you get the hang of it.

### Rails 2:

Example:

  ruby script/generate feature post title:string body:text published:boolean
  ruby script/generate scaffold post title:string body:text published:boolean
  rake db:migrate
  rake cucumber