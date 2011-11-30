require 'rake/rdoctask'
require 'rake/testtask'

desc 'Default: run unit tests'
task :default => :test

desc 'Run unit tests'
Rake::TestTask.new :test do |t|
  t.libs << 'test'
  t.pattern = 'test/**/*_test.rb'
  t.verbose = true
end

desc 'Generate RDoc documentation'
Rake::RDocTask.new :rdoc do |rdoc|
  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = 'Trashed'
  rdoc.options << '--line-numbers' << '--inline-source'
  rdoc.rdoc_files.include('MIT-LICENSE')
  rdoc.rdoc_files.include('README')
  rdoc.rdoc_files.include('lib/**/*.rb')
end