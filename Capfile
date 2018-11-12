# Load DSL and set up stages
require "capistrano/setup"
require "capistrano/deploy"

require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

require 'capistrano/rails'
require 'capistrano/rails/db'
require 'capistrano/bundler'
require 'capistrano/rvm'
require 'capistrano/puma'

install_plugin Capistrano::Puma

# Include tasks from other gems included in your Gemfile
 require "capistrano/rails/assets"
 require "capistrano/rails/migrations"

# Load custom tasks from `lib/capistrano/tasks` if you have any defined
Dir.glob("lib/capistrano/tasks/*.rake").each { |r| import r }
