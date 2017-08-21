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

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

$ git add .

$ git commit -m "Edit 3"
[master 02aff49] Edit 3
 1 file changed, 42 insertions(+)

BACKTRACK
$ git remote -v
origin  https://github.com/TekMason/testrepo1.git (fetch)
origin  https://github.com/TekMason/testrepo1.git (push)

$ git remote add upstream https://github.com/fusionpbxtest/testrepo1.git

$ git remote -v
origin  https://github.com/TekMason/testrepo1.git (fetch)
origin  https://github.com/TekMason/testrepo1.git (push)
upstream        https://github.com/fusionpbxtest/testrepo1.git (fetch)
upstream        https://github.com/fusionpbxtest/testrepo1.git (push)

$ git fetch upstream
From https://github.com/fusionpbxtest/testrepo1
 * [new branch]      master     -> upstream/master

$ git branch -va
* master                  02aff49 [ahead 1] Edit 3
  remotes/origin/HEAD     -> origin/master
  remotes/origin/master   500d9a4 Merge pull request #1 from TekMason/patch-1
  remotes/upstream/master 500d9a4 Merge pull request #1 from TekMason/patch-1

$ git checkout master
Already on 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

$ git merge upstream/master
Already up-to-date.

$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

$ git push
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 772 bytes | 772.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/TekMason/testrepo1.git
   500d9a4..02aff49  master -> master


