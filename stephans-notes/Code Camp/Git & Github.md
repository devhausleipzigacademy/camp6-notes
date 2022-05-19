# Git 
Git is a Version control system. 
It is a distributed control system (contrary to a centralized system)
Used by virtually all programmers

## Mindmap
<iframe width="768" height="432" src="https://miro.com/app/live-embed/uXjVO1mEfc8=/?moveToViewport=979,-55,3944,2092" frameBorder="0" scrolling="no" allowFullScreen></iframe>

## Functions 
- track changes
- swap versions
- undo changes
- great for team work (to exchange files easily and quickly between members)

## Git Structure
- Working Directory -> current version and root
- staging directory (.index) -> version and changes meant to be committed to repository
- Head -> pointer that keeps track of your location on version tree

![[Git Visualization.png]]

## Commands
These commands can be used in [[Bash]]
***
git init -> create fresh or reopen repository in folder you are currently in
git add (file) -> adds files or folders to staging directory
git status -> show changes and status of current repository
git commit -m "initial commit"-> commit flag -m for message followed by text important as description for change
git log -> shows the version history containing all changes to repository
git log --graph -> adds visualization to log
git help -> show information on git and commands
git fetch -> gets updated view of repository on remote server; follow by git status to compare online and local versions
git branch -> branches anzeigen, hinzufügen oder entfernen; flag -d to delete; flat -a to 
git pull -> gets latest repository version online and merges it with local version
git pull consists of both fetch and merge command 
git push -> pushes changes online to remote server so that team members and other can see changes and updates you made
git checkout -> switch branches
git rebase -> relocate branch and change version history to reflect that change; simiar to merge but without additional commit and dangerous as it changes history; useful for cleaning up history or redoing accidental commit
git clone SSHkey -> copies repository from remote source unto hard drive
git merge otherbranch -> merge otherbranch into current branch
git rm -> remove file from filesystem and from repository
git reset -> unstage changes

## Branches 
- branches can be used to work on different features and areas of a project and keep these work areas separate from each other and from live version
- to create and immediately switch to new branch use git checkout -b newbranch
- how to merge branches? Go to main branch, use git merge otherbranch to merge that branch with the one you are on

## Setting up the Remote
- either via terminal or via github
- folder .git contains remote information and needs to be updated to establish a connection
- common name for remote is origin

## Merge Conflicts & Pull Requests
- git push will fail if remote and local repository differ and cannot be reconciled
- need to perform git pull to solve conflict 
- auto merge will fail
- opening editor, e.g. nano will show merging conflict and allow for easy consolidation by removing conflict markers and making desired changes 	

## Cherrypicking
- checkout nameofbranch nameofile #to-do 

## Gitignore
