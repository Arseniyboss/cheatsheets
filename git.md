# git cheatsheet

## Saving Changes

| Command                        | Description                          |
| ------------------------------ | ------------------------------------ |
| git init                       | initialize a local repository        |
| git add .                      | add all changes to the staging area  |
| git commit -m [commit-message] | save the changes to local repository |

## GitHub Commands

| Command                          | Description                                                                                               |
| -------------------------------- | --------------------------------------------------------------------------------------------------------- |
| git clone [url]                  | create a local copy of a remote repository                                                                |
| git remote add origin [url]      | add a remote repository                                                                                   |
| git push -u origin [branch-name] | push the specified branch to remote repository and remember the branch                                    |
| git push                         | push the current remembered branch to remote repository                                                   |
| git push –all                    | push all branches to remote repository                                                                    |
| git pull origin [branch-name]    | fetch changes from the specified branch of the remote repository and merge them into the local repository |
| git pull                         | fetch changes from a remote repository and merge them into local repository                               |
| git pull --rebase                | use when git pull does not work                                                                           |
| git fetch                        | fetch changes from a remote repository                                                                    |

## Undoing Things

| Command                      | Description                                   |
| ---------------------------- | --------------------------------------------- |
| git checkout [commit-id]     | switch to the specified commit                |
| git revert [commit-id]       | delete the specified commit                   |
| git reset --hard [commit-id] | delete all commits after the specified commit |

## Branches and Merging

| Command                                           | Description                                        |
| ------------------------------------------------- | -------------------------------------------------- |
| git checkout -b [branch-name]                     | create the specified branch and switch to it       |
| git checkout [branch-name]                        | switch to an already existing branch               |
| git branch -m [old-branch-name] [new-branch-name] | rename a local branch                              |
| git merge [branch-name]                           | merge the specified branch into the current branch |
| git branch                                        | list local branches                                |
| git branch -a                                     | list local and remote branches                     |
| git branch -D [branch-name]                       | delete the specified branch                        |

## Viewing History

| Command           | Description                                                           |
| ----------------- | --------------------------------------------------------------------- |
| git status        | display the state of staging area                                     |
| git log           | display all commits including their text, id, branch, author and date |
| git log --oneline | display all commits on one line including their text, id and branch   |

## Editing Commits

| Command                                    | Action                                                  |
| ------------------------------------------ | ------------------------------------------------------- |
| git commit --amend -m [new-commit-message] | edits the last commit                                   |
| git rebase -i HEAD~n                       | lists the last n commits for editing in vim             |
| git rebase -i [commit-id]                  | lists commits after specified commit for editing in vim |
| git rebase -i --root                       | lists all commits for editing in vim                    |

### Using git rebase

1. replace **pick** with **reword** before each commit message you want to change
2. type the new commit message in each resulting commit file

### Making changes in vim

1. Press **i** to enter editing mode
2. Press **esc** to exit editing mode
3. Type **:wq** to save changes
4. Press **Enter** to exit vim
