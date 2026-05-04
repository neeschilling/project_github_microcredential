# Commonly used commands in git and GitHub

## Adding a ssh key for a new computer you wanna use Github on

1. Create a new ssh key for the new computer

`ssh-keygen -t ed25519 -C "your_email@example.com"`

2. copy the public ssh key to clipboard

3. Paste it into the ssh key section on Github

## Configurate git in new repository

1. Give username

git config --global user.name "Your Name"

2. Give E-mail adress

git config --global user.email "email"

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

