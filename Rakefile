require 'rubygems'

begin
  require "bundler/setup"
rescue Bundler::GemNotFound => e
  STDERR.puts e.message
  STDERR.puts "Try running `bundle install`."
  exit!
end

Bundler.require

Gemstub.test_framework = :rspec

Gemstub.gem_spec do |s|
  s.version = '0.3.0'
  s.rubyforge_project = 'magrathea'
  s.add_dependency('mark_facets', '>= 0.1.0')
  s.add_dependency('delayed_job', '< 3.0.0')
  s.email = 'mark@markbates.com'
  s.homepage = 'http://www.metabates.com'
end

Gemstub.rdoc do |rd|
  rd.title = 'DJ Remixes'
end


# git log --all --format='%aN' | sort -u