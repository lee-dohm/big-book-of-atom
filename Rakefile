require 'tmpdir'

GITHUB_REPONAME = "lee-dohm/big-book-of-atom"

desc 'Generate book'
task :generate do
  sh 'bundle exec middleman build'
end

desc 'Open the book locally'
task :open do
  sh 'open build/index.html'
end

desc 'Generate and push book to GitHub Pages'
task :push => [:generate] do
  Dir.mktmpdir do |tmp|
    cp_r 'build/.', tmp
    Dir.chdir tmp
    sh 'git init'
    sh 'git checkout -b gh-pages'
    sh 'git add .'
    message = "Site updated at #{Time.now.utc}"
    sh "git commit -m #{message.shellescape}"
    sh "git remote add origin git@github.com:#{GITHUB_REPONAME}.git"
    sh 'git push --force origin gh-pages'
  end
end
