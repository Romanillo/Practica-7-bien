$:.unshift File.dirname(__FILE__) + 'lib'

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new

task :default => :test
desc "Realiza los tests con formato deseado"

task :test do
   sh "rspec -Ilib spec/ppt_fraccionario.rb --format documentation"
end



desc "Test en formato html"
task :thtml do
  sh "rspec -Ilib spec/ppt_fraccionario.rb -f html > index.html"
end

