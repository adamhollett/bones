task :bundle do
  sh 'bundle --quiet'
end

task server: [:bundle, :clean] do
  sh 'bundle exec jekyll liveserve'
end

task :clean do
  sh 'bundle exec jekyll clean'
end
