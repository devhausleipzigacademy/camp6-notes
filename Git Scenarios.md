# Git Scenario

## Get new repo from remote, change something, commit, push changes to remote

- Go to Github, click on the repo, go to the "Code" dropdown, click on "SSH", copy the SSH URL

- Go to your shell
```sh
git clone git@github.com:organization/example-repo.git
```

The repo will be cloned as a folder with the same name as the repo in the current folder where you execute the command

- CD into the repo folder and open the folder in your code editor/edit files in your command line (i.e. VIM)

- Double check you are on the correct branch (i.e. a specific feature branch or the development branch, NOT production/main)
```sh
# Check status, i.e. current branch, changes to working dir, staged changes, last commit, etc...
git status

# List branches that are available locally
git branch

# List branches that are available locally + views of remote branches
git branch -a

# Switch to a specific branch
git checkout randomBranch

```

- Make changes to files (make sure to save the files!)

- Stage your changes
```sh
# stage everything in current directory
git add .

# stage a folder
git add randomFolder/

# stage a file
git add randomFile.js
```

- Commit your changes to your local version of the branch
```sh
# Pass the commit message inline
git commit -m "A description of the changes you made in this commit"

# Use your shell's standard code editor (probably VIM) to write the commit message
git commit
```

- Push your changes to the remote branch
```sh
git push
```


## Make new repo, push to remote, set up 'Gitflow' style branch structure, add feature branch, update main directly, update feature branch, merge feature branch into main

- Go into your projects folder, make a new folder for your project, make a new git repo
```sh
cd ~/projects

mkdir myNewProject

cd myNewProject

git init
```

- Go onto Github, create a new repo by clicking on the "New" repository button

- Click through, follow instruction given by Github to connect existing repo to the remote on Github

- Create Gitflow style branch structure
```sh
# Note: we already have a single branch, main; these are extra

# a branch for integrating features and testing
git checkout -b development

# we are now on 'development' branch
# push to remote
git push --set-upstream origin development

# create feature branches
git checkout -b feature1
git push --set-upstream origin feature1


git checkout -b feature2
git push --set-upstream origin feature2
```

- Simulate someone making a change to development after you created your feature branches
```sh
git checkout development
touch randomFileForExamplePurposes
git add .
git commit -m "Simulate someone else changing dev"

# Push changes to remote version of branch
git push
```

- Work on your feature
```sh
git checkout feature1

# simulate working on your feature
touch someSortOfMeaningfulWork
git add .
git commit -m "This is very valuable to the company"

# Push changes to remote version of branch
git push
```

- Pretend you don't know the dev branch has been changed; follow good practice
```sh
git fetch
git checkout dev
git pull
git log
# We'll see it's been updated
```

- Merge dev into your feature branch
```sh
git checkout feature1
git merge development

# Hopefully will auto-resolve, otherwise handle the merge conflicts
```

- Merge your feature branch into dev
```sh
git checkout development
git merge feature1

# will auto-resolve, since you've technically already handled the merging
```