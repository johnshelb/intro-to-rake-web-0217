desc 'requires environment'
task :environment do
  require_relative './config/environment'
end

namespace :greeting do

  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end


  desc 'outputs hola to terminal'
  task :hola do
    puts "hola de Rake!"
  end

end

namespace :db do

  desc 'migrate changes to database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seeds db'
  task :seed do
    require_relative './db/seeds'
  end

end
