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

`git log --oneline --graph --decorate --all` (can alias this to `git ll`)
* 17e6cea (HEAD -> master, origin/master, origin/HEAD, my_first_branch) start tut
* b3042d3 Initial commit

how to move HEAD to new branch?
`git checkout my_first_branch` but new git way is `git switch my_first_branch`

now `$ git log --oneline --graph --decorate --all` shows
* 5bdc106 (HEAD -> my_first_branch) commit on a branch
* 17e6cea (origin/master, origin/HEAD, master) start tut
* b3042d3 Initial commit

**Use [Daniel's FAQ with checklist](https://chendaniely.github.io/training_ds_r/help-faq.html)**

History:
```548  git commit -m "more branch notes"
549  git push origin my_first_branch
550  git branch
551  git switch master
552  git branch
553  cat README.md
554  git pull origin master
555  cat README.md
556  git remote -v
557  git branch -a
558  git log --oneline --graph --decorate --all
559  git branch -d my_first_branch
560  git log --oneline --graph --decorate --all
561  git fetch --prune
562  git log --oneline --graph --decorate --all
```

Exercise
- create new branch
- edit README
- add, commit
- git push origin <branch>
- PR
- merge and delete remote branch
- locally...
- Go back to master: git checkout master
- Pull down your merged code: git pull origin master
- Delete your branch: git branch -d my_awesome_task (note it is a lower case d)
- Clean up your branches: git fetch --prune
