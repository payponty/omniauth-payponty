# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
require './lib/omniauth-payponty/version.rb'
Jeweler::Tasks.new do |gem|

  gem.name = "omniauth-payponty"
  gem.homepage = "http://payponty.github.io/omniauth-payponty/"
  gem.license = "MIT"
  gem.summary = %Q{PayPonty lib for Omniauth.}
  gem.description = gem.summary
  gem.email = "payponty.info@gmail.com"
  gem.authors = ["PayPonty"]
  gem.version = OmniAuth::Payponty::VERSION

end
Jeweler::RubygemsDotOrgTasks.new

require 'rspec/core'
require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = FileList['spec/**/*_spec.rb']
end

task :default => :spec

require 'yard'
YARD::Rake::YardocTask.new
