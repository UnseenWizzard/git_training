# Git Training
_Adapted from Nice Reidman's interactive Git tutorial
["Learn git concepts, not commands"](https://dev.to/unseenwizzard/learn-git-concepts-not-commands-4gjc)_

# Local Version Control
<img src="./images/localVCS.png" height="400"/>

# Centralised Version Control
<img src="./images/cvcs.png" height="400"/>

# Distributed Version Control
<img src="./images/dvcs.png" height="500"/>

## Git Overview
<!-- ![](./images/teachingGit/1-dvcs.png) -->
<img src="./images/teachingGit/1-dvcs.png" width="700"/>

## Getting a Remote Repository
- Fork https://github.com/john-french/git_training
  - creates your own remote copy of a repository

- Get your copy of the remote repo onto your machine


```
git clone https://github.com/{YOUR USERNAME}/git_training.git
```

- creates a new directory called `git_training` on your machine


## Cloning a repository
<img src="./images/teachingGit/2-clone.png" width="700"/>

## Adding new things
- Move to the repo directory and add a new file

```
cd git_training
echo "This is Bob" > Bob.txt
```
- Check the status of your working directory
```
git status
```
<img src="./images/teachingGit/3-tracked-untracked.png" width="700"/>

## Adding new things

<img src="./images/teachingGit/4-add-commit-push.png" width="700"/>
