require 'rubygems'
require 'bundler'

Bundler.setup(:default, :development)

require 'rspec/core'
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec)

require 'rubocop/rake_task'
RuboCop::RakeTask.new(:rubocop)

task default: [:rubocop, :spec]

require 'rake'

Bundler::GemHelper.install_tasks

require 'gem_licenses'
Gem::Licenses.install_tasks
