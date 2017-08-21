# testrepo1
Just Testing

EDIT 1 with github pull request and no restrictions


EDIT 2 - FAIL
mkdir testrepo1
cd testrepo1
git init
git remote add upstream https://github.com/fusionpbxtest/testrepo1.git
git fetch upstream
git checkout master
 edit README.md (this file) and save

git status
git add .
git commit -m "edit2"
git status
 On branch master
 Your branch is ahead of 'upstream/master' by 1 commit.
   (use "git push" to publish your local commits)
 
 nothing to commit, working tree clean
git push
 remote: Permission to fusionpbxtest/testrepo1.git denied to TekMason.
 fatal: unable to access 'https://github.com/fusionpbxtest/testrepo1.git/': The requested URL returned error: 403


EDIT 3
Instructions from GitHub Standard Fork & Pull Request Workflow
https://gist.github.com/Chaser324/ce0505fbed06b947d962

go to https://github.com/fusionpbxtest/testrepo1
click Fork.  Creates https://github.com/fusionpbxtest/testrepo1

$ pwd
/c/Users/TekMason/gitroot

$ git clone https://github.com/TekMason/testrepo1.git
$ cd testrepo1
$ ls
README.md

 open README.md, make edits and save
 