Procedure
2017-08-21

Instructions from GitHub Standard Fork & Pull Request Workflow
https://gist.github.com/Chaser324/ce0505fbed06b947d962

Go to the original repo
Creates https://github.com/fusionpbxtest/testrepo1
Click Fork

go to gitroot
$ pwd
/c/Users/TekMason/gitroot

$ git clone  https://github.com/TekMason/testrepo1.git
$ cd testrepo1
$ git remote add upstream https://github.com/fusionpbxtest/testrepo1.git
 do a check 
$ git remote -v

$ git fetch upstream
$ git branch -va
$ git checkout master
$ git merge upstream/master

...

EDIT FILES
$ git status
$ git add .
$ git commit -m "Commit Message Here"
$ git push

Go to GitHub repo and should see changes
Do a pull request

...

time goes by...

SYNCHRONIZE FROM SOURCE REPO

# Fetch from upstream remote
$ git fetch upstream

# View all branches, including those from upstream
git branch -va

# Checkout your master branch and merge upstream
git checkout master
git merge upstream/master

git push

....
good to go with new edits (EDIT FILES)

On original select what?
Merge your pull request (1 edit gave 2 commits)
Squash and merge
Rebase and Merge






