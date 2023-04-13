# 20230408: git_collaboration

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
- 'git fetch': update the git log
	- 'git fetch --prune': remove any remote branches that have been deleted from the git log
- 'git branch -d <NAME>': delete the branch <NAME> local


- pull requests will auto update when you push changes to the branch


Changes to readme on conflict 1