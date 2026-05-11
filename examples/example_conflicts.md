# Examples of conflicts
Document examples of conflicts and their resolution here. 

*Hint: git usually tells you what needs to be done when an issue arises. Make sure to read the output in the terminal and follow the steps suggested.*

## Example 1

### Conflict situation
I am trying to push some changes to the remote repository but I get an error:

```
$ git push
To https://github.com/neeschilling/project_github_microcredential.git
 ! [rejected]        merge_branch_2 -> merge_branch_2 (fetch first)
error: failed to push some refs to 'https://github.com/neeschilling/project_github_microcredential.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

### Conflict resolution
Because we were both working on the same file, the person trying to push last will get an error. You first need to check which changes were made by both and which to keep. This can be done with the command  `git config pull.rebase false`  after which you peform `git pull`.  
This will now open the file involved in editing mode you can see the conflicting changes, decide what to keep and what not (or keep everything) after which you can add, commit and push the final changes.