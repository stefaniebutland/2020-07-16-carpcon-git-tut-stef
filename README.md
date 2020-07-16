# 2020-07-16-carpcon-git-tut-stef
Carpentry Con git workshop with Daniel Chen

`open .` opens Finder in that dir
`xdg-open .` does a thing with folders?

`git clone <url>`


## Branches
`git branch`
* master
  my_first_branch

`git branch -a`
* master
  my_first_branch
  remotes/origin/HEAD -> origin/master
  remotes/origin/master

`git log --oneline --graph --decorate --all`
* 17e6cea (HEAD -> master, origin/master, origin/HEAD, my_first_branch) start tut
* b3042d3 Initial commit

how to move HEAD to new branch?
`git checkout my_first_branch` but new way is `git switch my_first_branch`
