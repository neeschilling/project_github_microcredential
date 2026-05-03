# Commonly used commands in git and GitHub

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

