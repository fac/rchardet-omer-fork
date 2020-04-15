require "bundler/gem_tasks"
require "rspec/core/rake_task"
begin
  require 'lib/rchardet'
rescue LoadError
  module CharDet; VERSION = '0.0.0'; end
  puts "Problem loading rfeedparser; try rake setup"
end

RSpec::Core::RakeTask.new(:spec)

task :default => :spec
