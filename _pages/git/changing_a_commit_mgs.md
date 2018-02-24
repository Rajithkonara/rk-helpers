---
layout: default
---

- changing most recent commit message - commit not push to github

    `
         git commit --amend
    `
- pused to repo most recent commit, 
   follow above steps and 

    `
         git push --force branch-name
    `

- changing commit message for older or multiple commits
    
    List last n commits

    `
        git rebase -i HEAD~n
    `

- push with --force
