namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end
end

desc 'runs pry'
task :console => :environment do
  Pry.Start
end

desc 'building environment'
task :environment do
  require_relative './config/environment'
end

namespace :db do

  desc 'Migrates the stuff'
  task :migrate => :environment do
  end

  desc 'seed the database w/ dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

end
