require "bundler/gem_tasks"

gemspec = eval(File.read("longbow.gemspec"))

task :build => "#{gemspec.full_name}.gem"

file "#{gemspec.full_name}.gem" => gemspec.files + ["longbow.gemspec"] do
  system "gem build longbow.gemspec"
end