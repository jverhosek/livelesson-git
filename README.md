#GIT Notes
- 'git init': initialize current folder as a git repo
- 'git clone <URL>': brings the git repo from <URL> to current folder 
- 'git status' tells us what we need to know about our current repo and its state
- 'git add <FILE>': adds <FILE> to the staging area
- 'git commit': opens up a text editor to write a commit message
	-'git commit -m "MESSAGE"' : writes MESSAGE as a commit without a text editor
- 'git log': shows the of our commits
	-'git log --oneline': shows the shorter oneline commit
- 'git diff': compare current uncommitted state with last known git state
	-'git diff --staged': runs git diff between the staging areas and last known state
- 'git diff HEAD~<NUMBER> : compares HEAD with commit <NUMBER> ago (relative)
- 'git diff <HASH>':  compares HEAD with the commit in <HASH>
- 'git restore --source <HASH OR HEAD~> <FILE>' : restore file to <HASH OR HEAD~>
	- 'git checkout <HASH OR HEAD~> <FILE>' : restores file to <HASH OR HEAD~>
		- 'git checkout <HASH OR HEAD~>: if you forget the file, you end up in detach>
		- 'git checkout main': go back to main
		- 'git switch main': go back to main
#remotes
- 'git remote add <NAME> <URL>': adds the <URL> as a remote with the name <NAME>
	-<NAME> is by cinvention callled 'origin'
- 'git remote -v: look at all the remotes you have
-'git push <WHERE> <WHAT>: pushes the <WHAT> branch to <WHERE>
	'git push origin main'
- 'git pull <WHERE> <WHAT>': pulls the <WHAT> branch in <WHERE> to local computer
