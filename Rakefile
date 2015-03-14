require "bundler/gem_tasks"

desc 'Build and copy Mocha and Chai assets from submodules into vendor/assets'
task :assets => ['assets:copy']

namespace :assets do
  task :copy do
    sh 'git submodule update --init'
    mkdir_p 'vendor/assets/javascripts'
    cp 'flatjs/flat.js',  'vendor/assets/javascripts/'
  end
end

