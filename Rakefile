namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc "hello en Espanol"
  task :hola do
      puts "hola de Rake!"
  end

  desc "hello am Deutsch"
  task :guten_tag do
    puts "guten tag von Rake!"
  end
end

namespace :db do 
  desc "migrate changes to your database"
  task :migrate => :environment do
    Student.create_table
  end

  desc "seed with dummy data"
  task :seed do
    require_relative './db/seeds.rb'
  end

end

task :environment do
  require_relative "./config/environment.rb"
end

desc "drop into pry console"
task :console => :environment do 
  Pry.start
end