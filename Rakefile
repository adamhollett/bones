task default: :server

task server: :clean do
  sh 'bundle exec jekyll liveserve'
end
task s: :server

task :clean do
  sh 'bundle exec jekyll clean'
end
