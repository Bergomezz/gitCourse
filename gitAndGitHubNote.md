# **_Some notes of the git course for the future_**

- `git --version` - just to see the version that you using
- `git init` - to initialize the git repository
- `git add` - adds files to staging area (stage)
- `git commit` - commits staged changes into local repository history
- `git push` - push the staged change into remote repositories
- `git remote` - synchronize the local repository with the online host repository
- `git remote show` - If you use with origin, it will show a lot of details information about all branch
- `git branch` - locate and list the branches. If you using the flag `-d`, you will delete only the branch that you already merge and if you use the flag `-D`, you will force delete the branch. With the flag `-a`, we can list all branch local and remote. With the flag `-c`, we can create a new branch. With the flag `-r`, we can visualize the remote branch. With the `-vv` flag, list local tracking branches and their remotes.With the flag `--track`, you can make a tracking local branch with the remote one. It's a good practicing to use the same name branch as the remote one. Using `--delete --remotes`, you can delete the remote branch.
- `git checkout` - change into the branches, if you use with the flag `-b` you will create a new branch and change for it
- `git merge` - merge branches
- `git switch` - new command to change between branches
- `git rm` - remove some added information that you unstage the file
- `git restore` - going back to the head branch and "stash" the modification that you made and unstage the file that you already added
- `git clean` - new command that could remove the untracked file with the flag `-dn` ou with `-df` to force the remove command
- `git reset` - copy the latest change the would committed before the change. using the command + `HEAD~1`, you return to the latest commit in the HEAD. If you do with `--hard`, you will delete the commit and the file staged
- `git ls-file` - list the already file that you staged in your repo
- `git log` - log all you commit and id for you to use
- `.gitignore` - a file that you could put all the files that you can't send to the repo. If you use '!' before the name of the file, you could make some exception and send that specific file to the repo. <br> Example: If you use the `*.doc`, this is ignore all file that end with .doc, but if you want to send some specific file .doc, you need to put `!fileName.doc`. This will make the file be ready to stage and send to the repo
- `git reflog` - Allow us to bring back kind of lost information, related to commits or to branches (A log og all project changes made including deleted commits)
- `git merge --no-ff` - Automatic merge the branch and left individually path in recursive mode
- `git rebase` - Merge two branches and create another commit with all commit made before (Change the base (i.e the parent commit) of commits in another branch)
- `diff --cc branch_name/file_name` - This is show the difference between the 2 commits to choose what is accepted
- `git merge --abort` - Used to abort the merge to recheck the diff
- `git cherry-pick` - Used with the commit id to merge only the specific commit to the selected branch (Copy commit including the changes made only in this commit as _***HEAD***_ to other branch)
- `git tag` - Used to tag some selected commit to be easier to identify the commit id that was did it
- `git stash` - Temporary storage for unstaged and uncommitted changes
- `git fetch` - Adding with origin, it will bring all you have of your remote repository

<br>

- ## **Some note of command line commands from Mac and Unix OS**

- `mv` - use to move and rename the folder/file
- `touch` - create a file
- `cp` - copy file/folder
- `rmdir` - remove folder
- `clear` - clear the terminal
- `echo` - could be use to create and pass text to the file
- `cat` - print what information is inside of the file

If you have some question and want to know more, use the `man` and the command that you want to know and the flags that you can used for

<br>

## **Some note of commands line command from cmd**

- `cd /` - navigate directly from the root directory
- `cls` - clear the terminal
- `echo` - create a file
- `type` - equal as the cat on the Mac and Unix OS
- `del` - delete file from the folder
- `rmdir` - delete the folder
- `copy` - copy file and folder
- `move` - move file and folder

<br>
<br>

## **How to handling whit merge conflicts**

> [!NOTE]
>
> - Compare Changes - Accept Current Change - Accept the Incoming Change - Accept Both Change
>
> > 1.  You will need to check what is the best option for the correction and made the change
