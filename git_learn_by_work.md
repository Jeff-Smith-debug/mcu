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
$ git push -u origin（别名） master 
# 将-u后面两个变量变成了默认值，以后可以直接git push  默认就是 -u设置的内容

```

# 2 Alias for git
```bash
   alias gl='git pull'
   alias gaa='git add .'
   alias gcmsg='git commit -m'
   alias gcam='git commit -a -m'
   alias gp='git push'
   alias gco='git checkout'
   alias gm='git merge'
   alias gss='git status -s'
   alias glol='git log –graph –pretty = format:’%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset’ –abbrev-commit'
   alias grh='git reset HEAD'
   alias gba='git branch -a'
   alias gcf='git config –list'
   alias gcl='git clone –recursive'
   alias gd='git diff'
   alias ghh='git help'

   alias ns='npm run serve'
   alias nb='npm run build'
   alias nd='npm run dev'

```
Problem-2 I have modified the .bashrc file,but every open git bash,must source ~/.bashrc
```solve
vi ~/.bash_profile 在文件内部输入:
# Loading .bashrc File
source ~/.bashrc # 在 .bash_profile 文件中自动加载 .bashrc 文件.

```

