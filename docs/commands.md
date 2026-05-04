# Commonly used commands in git and GitHub

## Adding a ssh key for a new computer you wanna use Github on

1. Create a new ssh key for the new computer

`ssh-keygen -t ed25519 -C "your_email@example.com"`

2. copy the public ssh key to clipboard

3. Paste it into the ssh key section on Github

## Configurate git in new repository

1. Give username

`git config --global user.name "Your Name"`

2. Give E-mail adress

`git config --global user.email "email"`

## When you start a new repository locally 

1. Make a folder where the project will be stored 

2. In the commandline go to the folder 

`cd <folder_adress>`

3. Initialize git

`git init`

4. Save your first file into the folder

5. Add file to repository

`git add <filename>`

6. Commit together with a meaningful message

`git commit -m <meaningful_message>`

## Connecting your local repositroy to GitHub for the first time

1. Add the repository to you GitHub account using a ssh adress 

`git remote add origin <ssh_address>`

If you accidentally added a wrong address, you can remove with this command

`git remote remove origin`

2. Set the name of the main branch 

`git branch -M <main_branch_name>`

3. Push your changes to GitHub while setting upstream

`git push --set-upstream origin <main_branch_name>`

## Check git status

Shows branch you are in and potential untracked changes

`git status`

Shows history of all changes together with ID

`git log`

Compare commits

`git diff`

`git show`

## Recover to a previous state

Recover to a previous state: Removes changes (means also deleting IDs so you can no longer access)

`git reset`

Reverts to previous state: Adds revert as a new head which means all changes are still tracked

`git revert`

Rewrite last commit message

`git commit -amend`

Go to a specific ID (!Warning tracks will not be saved unless you attach the new branch to main)

`git checkout <commit_ID>`

Attach branch

`git switch -c <new_branch_name>`

## Alternative history

Make new branch

`git branch <branch_name>`

Go to specific branch

`git checkout <branch_name>`

Merge branches

`git merge <target_branch_name>`

Remove branch

`git branch -d <branch_name>`

## Tagging

To highlight good versions

`git tag <name>`

`git push --tags`





