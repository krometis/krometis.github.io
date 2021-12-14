To make an update:
```
#Switch to the source branch
git checkout source

#Make changes, e.g.,
vi _config.yml
vi _pages/projects.md 
vi _bibliography/papers.bib

#Deploy locally (generates _site/)
bundle exec jekyll serve

#Add, commit, push changes (to the source branch)
git add -A
git commit -m 'source: updated X, Y, Z'
git push origin source

#Switch to master branch
git checkout master

#Copy contents of _site into root of website
#May also need to remove files that were removed, etc
cp -r _site/* .

#Add, commit, push changes (to the source branch)
git add -A
git commit -m 'master: updated X, Y, Z'
git push origin master
```

To set up (on Ubuntu via [WSL](https://docs.microsoft.com/windows/wsl/)):
```
#Jekyll instructions say not to install centrally, so ran 
#these and added to .bash_profile
export GEM_HOME="$HOME/gems"
export PATH="$GEM_HOME/bin:$PATH"

#Had to do this once to get apt-get to find packages
sudo apt-get update

#Install dependencies
sudo apt-get install ruby-full build-essential zlib1g-dev

#Add Jekyll
gem install jekyll bundler

#Add missing gems
bundle install
```
