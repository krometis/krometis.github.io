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
cp -r _site/ .

#Add, commit, push changes (to the source branch)
git add -A
git commit -m 'master: updated X, Y, Z'
git push origin master
```
