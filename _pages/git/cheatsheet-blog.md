---
layout: default
---
Configurations
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|Show git configs               |  `git config --list`                              |
|Show username                  |  `git config --global user.name`                  |
|Set username                   |  `git config --global user.name "username"`       |
|Show email                     |  `git config --global user.email`                 |
|Set email                      |  `git config --global user.email "email"`         |

Remotes
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|List remotes                   |  `git remote -v`                                  |
|List remote branches           |  `git ls-remote --heads origin`                   |
|Add a remote                   |  `git remote add <remote-name> <remote-url>`      |
|Remove a remote                |  `git remote rm <remote-name>`                    |

Commit
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|Check Untracked Files          |  `git status`                                     |
|Git add untracked file         |  `git add $filename`                              |
|Git add all                    |  `git add .`                                      |
|Git commit                     |  `git commit -m "commit message"`                 |
|Git push                       |  `git push <remote-name> <remote-branch>`         |
|Git commit to previous commit  |  `git commit --amend`                             |
|Git pull from remote           |  `git pull <remate-name> <branch-branch>`         |
|Git rebase with remote         |  `git pull --rebase <remote-name> <branch-name>`  |

Branch
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|Show current branch            |  `git branch`                                     |
|Show remote branch             |  `git ls-remote --heads origin `                  |
|Git add new local branch       |  `git branch <branch-name>`                       |
|Git checkout to branch         |  `git checkout <branch-name>`                     |
|Git create and checkout        |  `git checkout -b <branch-name>`                  |
|Delete a local branch          |  `git branch -d <branch-name>`                    |
|Delete a remote branch         |  `git push origin --delete <branch_name>`         |

Diff
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|Git diff file                  |  `git diff $filename`                             |
|Git diff two revision          |  `git diff $sha1 $sha2`                           |
|Git diff only file name        |  `git diff --name-only $sha1$sha2`                |
|Compare git diff after commit	|  `git diff --cached`                              |
|Compate branches               |  `git diff <branch_1> <branch_2>`                 |

Log
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|Git log                        |  `git log --oneline`                              |
|Log with status                |  `git log --stat`                                 |
|Formatted output               |  `git log --pretty=format:"%h - %an, %ar : %s"`   |

Tag
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|List tags                      |  `git ls-remote --tags`                           |
|Create a tag                   |  `git tag <tagname>`                              |
|Push a tag to remote           |  `git push origin --tags`                         |
|Fetch tags                     |  `git fetch --tags`                               |
|Checkout to a tag              |  `git checkout tags/<tag_name>`                   |
|Delete a tag local             |  `git tag -d <tagname>`                           |
|Delete a tag remote            |  `git push --delete origin <tag_name>`            |

Clear
---------------------

|Description                    | Command                                           |
|---                            |---                                                |
|View what files will delete    |  `git clean -n`                                   |
|Clean/delete files             |  `git clean -f`                                   |
|Stash your local changes       |  `git stash`                                      |
|View stash list                |  `git stash list`                                 |
|Apply a stash (local changes)  |  `git stash apply`                                |