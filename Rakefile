require 'bundler'
Bundler::GemHelper.install_tasks

require 'spree/testing_support/extension_rake'
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new

task default: [:spec]

desc 'Generates a dummy app for testing'
task :test_app do
  ENV['LIB_NAME'] = 'solidus_recently_viewed'
  Rake::Task['extension:test_app'].invoke
end
