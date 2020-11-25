---
title: 04 - Git
created: '2020-11-17T13:36:46.365Z'
modified: '2020-11-17T14:06:17.828Z'
---

# 04 - Git
## Git design goals
- Speed
- Simplicity
- Strong branch/merge support
- Distributed
- Scales well for large projects

## Git configuration
- System level: `git config --system`
- User level: `git config --global`
- Repo level: `git config`

## Git areas
- Working directory
- Staging area
- Committed History
- Development branches

## Git tagging
Tags are simple pointers
- `git tag -a name -m message`

## Git initialize repo
`git init`

## Git clone repo
`git clone url`

## Git inspect the stage
`git status`

## Git inspect a commit
`git log`

## Git undoing
- Modified, not staged
  + `git checkout HEAD <<FILE>>`
- Modified, staged
  + `git reset HEAD <<FILE>>`
- Staged and not staged
  + `git reset HEAD --hard`
- Clean up untracked files
  + `git clean -f`
- Undo commit
  + `git reset HEAD~1`
  + `gir revert <<SHA1>>` (Creates revert commit)

## Git ammending
Add the current stage to prev commit
- `git commit --amend`

## Git branches
- `git checkout -b NAME`
- `git branch -d NAME`
...

## Git merge types
- Fast forward
- 3-way merge

## Git rebase
Moving a branch to a new base
`git rebase master`

## Git remotes
`git remote -v`
`git fetch; git merge` = `git pull`
`git push`

## Git remote workflows
- Centralized
  + Individual devs work on local repo and push to central repo
- Integrator
  + Everyone has local and public repo, useful for very large open-source projects

## Porcelain vs plumbing commands
- Porcelain: User friendly commands for everyday use
- Plumbing: Normally not used but building blocks of porcelain ones

## Examples of plumbing commands
- `git cat-file`
- `git hash-object`
- `git count-objects`

## Git Objects
- blob
- tree
- commit
- annotated tag

## What are branch and head (low level)
Pointer to a commit and pointer to a pointer
