namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
  desc 'outpts hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'does a migration'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'requires seed file'
  task :seed do
    require_relative "./db/seeds.rb"
  end
end

desc 'requires the environment file'
task :environment do
  require_relative "./config/environment"
end

desc 'exists'
task :console do
    puts "I am console"
end