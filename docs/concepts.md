# Git concepts

Git is a version control software to track changes in files over times which runs **locally** in contrast with github which is an **online** platform to store (backup) your Git repositories. This will allow you to easily share and collaborate with others. 

## Conceptual areas

1. Developing area: directory where the project is developed.
2. Staging area: in this space we organise files before a commit e.g. we want to commit file A and B together because they are related so we will put them both in the staging area.
3. Local repository: this is .git file where the git software manages all the versions that are committed.

## Commit messages

Adding a commit message is obligated, without it you cannot commit. **Adding conflict**

Be as descriptive as you can. You can use the following questions to write a meaningful message:

- Why was it changed?
- How does this address the issue?
- Are there any effects due the change?
- Are there any limitations of the change?

## From local to remote

- SSH key: A way to securely connect to a remote computer/location/server. We add it to github in the settings for ssh key.
- How to create an empty remote repository on github: add a new repository on github, give it a nice name, don't add any files and follow the instructions to connect with the local
- Before we can backup our local repository we need to connect it to the remote repository. This is done by adding the origin of the remote repository by using remote add origin. Setting up this connections (bridge) between both is only done once.
- I should always synchronise the changes. Git push will send changes to my collaborators and the remote repository while git pull will send the changes from my collaborators or online changes to to my local repository.

## README file

This is a detailed description of the project, usage and installation. If it is named like this, it will automatically be the first page the user sees.

## .gitignore file
A list of files that should be ignored. Usually this is data, backups, intermediate files and confidential files. You can also use regex to ignore files that contain the certain pattern. If you put .gitignore itself in the file, this will also be ignored. 

## Branching & checkout

To experiment risk free we can use branches. A new branch will have an independent timeline. It could be useful for debugging and testing especially when collaborating. You can move between the branches by using git checkout.
TIP: put the initial of the person who's working the branch in the name. 

### Mirror effect
When using multiple branches, your environment becomes dynamic. 

## Tagging
This is a way to highlight good versions (states/commits). It doesn’t matter in which branch. This way you don’t need to remember the commit id, but you can just give it a name. This is used e.g. for:
- A good version
- A version for a release
- A specific feature
- Experiment risk free
- ...