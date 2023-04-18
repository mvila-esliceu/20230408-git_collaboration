# 20230408: GGGGit Collaboration


## Creating a local repository
- 'git clone <URL>': downloads  the repo to your current directory
- 'git init'"initializes the current directory as a git directory



## Working with branches
- 'git branch <NAME>': creates a branch <NAME> where HEAD is
- 'git branch -a': list all branches you have, showing the one you are pointing to with a *
- 'git switch <NAME>': moves HEAD / switches you to the branch <NAME> 
	- 'git checkout <NAME>': "older" command to switch branches
	
	

## Exercise 2
- create a branch 'branch_defs'
- edit README
	- 'git log --oneline --graph --all'
	- 'git push'
	- pull request
- add/commit changes
- push branch
- create the PR
- merge the PR
- sync our local 'main' with 'origin/main'
- 'fech --prune'
- delete local branch



## Merging Branches
- 'git log --oneline --graph --all': show you a decorated hisotry log, your best friend (along with 'git status')
- 'git push <WHERE> <WHAT>': 'git push origin main' send branch 'main' to  remote 'origin'
- 'git pull <WHERE> <WHAT>': similar to 'push' but goes from remote to local computer

## Cleaning up brnaches + history
- 'git fetch': update the git log
	- 'git fetch --prune': remove any remote branches that have been deleted from the git log
- 'git branch -d <NAME>': delete the branch <NAME> local


- pull requests will auto update when you push changes to the branch


## Rebase
- 'git fetch --prune'
- 'git switch main'
- 'git pull origin main'
- 'git switch conflict_2'
- 'git rebase main'
- 'git rebase': command to change history, we are using it to fix conflict
	- 'git rebase --abort': go back to before you typed 'git rebase main'



## Git Flow

- https://www.atlassian.com/git/tutorials/syncing
- https://www.atlassian.com/git/tutorials/comparing-workflows


A convention people use for branches to separate "main"/"production" from "development" code


## Extras

- Problem: I just want my files to be somewhere else (commit)
	- solutions: 'git reset --hard <HASH>' --> move HEAD and the branch you are on to wherever you specified <HASH>
	
	
- Problem: I want to enforce a branch workflows
	- solution: settings > branches > branch protection rule
	- Note: if you are on your own, un-check review from 1 person
	
