# the MD aims to record the practical usage when I use git work.

Problem-1: git clone github-https,however we can know that we clone only onebranch-main by git branch(git branch -a),how to Syc other origin branch?
```git
$ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/master
$ git checkout -b master origin/master
Switched to a new branch 'master'
branch 'master' set up to track 'origin/master'.

$ git branch -a
  main
* master
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/origin/master

```
