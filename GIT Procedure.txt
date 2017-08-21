Procedure

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

 edit files
$ git status
$ git add .
$ git commit -m "Commit Message Here"
$ git push
