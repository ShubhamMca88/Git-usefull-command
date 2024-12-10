# Git and GitHub Guide

This guide provides a quick reference for common Git and GitHub commands.

## GitHub CLI

**Authentication**

*   `gh auth login`: Authenticate with your GitHub account.
*   `gh auth refresh -h github.com -s delete_repo`: Refresh your authentication token with delete repository permissions.

**Repository Management**

*   `gh repo list --full-name`: List all repositories with their full names.
*   `gh repo create <repo_name> --public/private --description "demo test"`: Create a new public or private repository with a description.
*   `gh repo delete <username>/<repository-name>`: Delete a repository.


## Git Commands

**Configuration**

*   `git --version`: Check your Git version.
*   `git config --global user.name "Your Name"`: Set your global username.
*   `git config --global user.email "your.email@example.com"`: Set your global email address.

**Initialization**

*   `git init`: Initialize a new Git repository.
*   `git config --global init.defaultBranch main`: Set the default branch name to "main" for new repositories.
*   `git branch -m main`: Rename the current branch to "main".

**Staging and Committing**

*   `git add .`: Stage all changes in the current directory.
*   `git commit -m "Initial commit"`: Commit staged changes with a message.
*   `git commit -am "Your commit message here"`: Stage all changes to tracked files and commit with a message.

**Pushing Changes**

*   `git remote add origin <repo_url>`: Add a remote repository.
*   `git push -u origin main`: Push local commits to the remote repository and set up tracking.

## Basic Git Commands

*   `git init`: Initializes a new Git repository.
*   `git clone <url>`: Clones an existing repository from a URL.
*   `git status`: Shows the status of changes in the working directory.
*   `git add <file>`: Stages a file for the next commit.
*   `git add .`: Stages all changes in the current directory.
*   `git commit -m "message"`: Commits staged changes with a message.
*   `git push`: Pushes committed changes to a remote repository.
*   `git pull`: Fetches and merges changes from a remote repository.
*   `git fetch`: Downloads objects and refs from another repository.
*   `git merge <branch>`: Merges a specified branch into the current branch.
*   `git branch`: Lists branches in the repository.
*   `git branch <branch-name>`: Creates a new branch.
*   `git checkout <branch>`: Switches to a different branch.
*   `git checkout -b <branch-name>`: Creates and switches to a new branch.
*   `git log`: Shows the commit history.
*   `git diff`: Shows changes between commits or between the working directory and index.
*   `git reset <file>`: Unstages a file.
*   `git reset --hard <commit>`: Resets the working directory and index to a specified commit, discarding changes.
*   `git rm <file>`: Removes a file from the working directory and stages the deletion.
*   `git stash`: Stashes changes for later use.
*   `git stash apply`: Re-applies stashed changes.
*   `git tag <tag-name>`: Tags a specific commit.

## Advanced Git Commands

*   `git rebase <branch>`: Reapplies commits on top of another base tip.
*   `git cherry-pick <commit>`: Applies a specific commit from one branch to another.
*   `git reflog`: Shows a log of references for the repository.
*   `git bisect`: Helps find the commit that introduced a bug.
*   `git archive`: Creates a tar or zip archive of files from a repository.
*   `git clean -f`: Removes untracked files from the working directory.