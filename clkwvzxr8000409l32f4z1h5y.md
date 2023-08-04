---
title: "Git Cheat Sheet: A Quick Reference Guide📖🚀"
datePublished: Fri Aug 04 2023 17:55:55 GMT+0000 (Coordinated Universal Time)
cuid: clkwvzxr8000409l32f4z1h5y
slug: git-cheat-sheet-a-quick-reference-guide
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1691080760278/34ef01f7-fe4a-4a77-9659-44f236be9477.jpeg
tags: github, git, devops, trainwithshubham

---

## Introduction 🌟

Version control systems are a crucial part of modern software development, and Git has emerged as the most popular choice for managing code repositories. Whether you're a seasoned developer or just starting with Git, having a handy cheat sheet can make your version control journey smoother. In this blog post, we'll provide a comprehensive Git cheat sheet containing essential commands and advanced techniques to boost your productivity. Let's dive in! 💻

## 🛠️ **Configuring Git:**

* `git config --global` [`user.name`](http://user.name) `"Your Name"`: Set your name for commit attribution.
    
* `git config --global` [`user.email`](http://user.email) `"`[`your@email.com`](mailto:your@email.com)`"`: Set your email for commit attribution.
    
* `git config --global core.editor "editor"`: Set your preferred text editor for commit messages.
    
* `git config --global --list`: List your Git configurations.
    

## 🏗️ **Creating and Cloning Repositories:**

* `git init`: Create a new Git repository in the current directory.
    
* `git clone <repository_url>`: Clone an existing repository to your local machine.
    

## 🔄 **Basic Git Workflow:**

* `git status`: Check the status of your working directory and see which files are modified.
    
* `git add <file>`: Add a specific file to the staging area (index) for the next commit.
    
* `git add .`: Add all modified files to the staging area for the next commit.
    
* `git commit -m "Commit message"`: Commit the changes in the staging area with a descriptive message.
    
* `git log`: View the commit history.
    
* `git diff`: Show the differences between your working directory and the last commit.
    

## 🌿 **Branching and Merging:**

* `git branch`: List all branches in the repository.
    
* `git branch <branch_name>`: Create a new branch with the given name.
    
* `git checkout <branch_name>`: Switch to the specified branch.
    
* `git checkout -b <branch_name>`: Create and switch to a new branch.
    
* `git merge <branch_name>`: Merge the changes from the specified branch into the current branch.
    

## 📤 **Updating and Publishing Changes:**

* `git pull`: Fetch and merge changes from the remote repository into the current branch.
    
* `git push`: Push your local commits to the remote repository.
    
* `git remote -v`: View the list of remote repositories.
    
* `git remote add <name> <repository_url>`: Add a new remote repository.
    

## ⚔️ **Resolving Conflicts:**

* Conflicts may occur during a merge or rebase. Open the conflicting file, resolve the conflicts manually, save the changes, and then use:
    
    * `git add <file>`: Add the resolved file to the staging area.
        
    * `git commit`: Commit the resolved changes.
        

## ↩️ **Undoing Changes:**

* `git reset HEAD <file>`: Unstage changes for a specific file, keeping the changes in your working directory.
    
* `git checkout -- <file>`: Discard changes in a file and revert it to the last committed state.
    
* `git revert <commit>`: Create a new commit that undoes the changes introduced by the specified commit.
    

## 🌐 **Working with Remotes:**

* `git fetch`: Fetch changes from the remote repository without merging them.
    
* `git remote show <remote_name>`: Show information about a specific remote repository.
    
* `git push <remote_name> <branch_name>`: Push the specified branch to the remote repository.
    
* `git push --force`: Forcefully push changes, potentially overwriting history (be cautious!).
    
* `git pull --rebase`: Fetch and rebase your local branch with the remote branch.
    
* `git remote rename <old_name> <new_name>`: Rename a remote repository.
    

## 🌟 **Advanced Branching and Merging:**

* `git rebase <branch_name>`: Rebase the current branch onto the specified branch.
    
* `git rebase --interactive <commit>`: Perform an interactive rebase, allowing you to squash, edit, and reorder commits.
    
* `git cherry-pick <commit>`: Apply the changes introduced by the specified commit to the current branch.
    
* `git reflog`: View the history of branch references, useful for recovering lost commits.
    

## 👥 **Collaborating with Others:**

* `git log --author="Author Name"`: View the commit history for a specific author.
    
* `git blame <file>`: See who made the last changes to each line of a file.
    
* `git clone --depth 1 <repository_url>`: Clone a repository with only the latest commit (shallow clone).
    
* `git push --set-upstream <remote_name> <branch_name>`: Set the upstream branch for your local branch.
    
* `git pull --rebase`: Fetch and rebase your local branch with the upstream branch (avoids unnecessary merge commits).
    

## 🏷️ **Working with Tags:**

* `git tag`: List all tags in the repository.
    
* `git tag <tag_name>`: Create a new lightweight tag at the current commit.
    
* `git tag -a <tag_name> -m "Tag message"`: Create an annotated tag with a message.
    
* `git push --tags`: Push all tags to the remote repository.
    

## 🎨 **Git Configurations:**

* `git config --global alias.<alias_name> <git_command>`: Create a custom Git alias.
    
    * Example: `git config --global` [`alias.co`](http://alias.co) `checkout` will allow you to use `git co` as a shorthand for `git checkout`.
        
* `git config --global core.ignorecase true`: Set Git to be case-insensitive (useful for Windows or macOS).
    
* `git config --global core.autocrlf true`: Automatically convert line endings during commit and checkout (useful for cross-platform collaboration).
    

## 🗑️ **Removing and Cleaning Up:**

* `git rm <file>`: Remove a file from the repository and the working directory.
    
* `git clean -n`: Dry-run to show what will be removed with the next git clean command.
    
* `git clean -f`: Remove untracked files from the working directory.
    

## Conclusion 🎉

With this comprehensive Git cheat sheet at your disposal, you're equipped to handle various version control tasks confidently. Git's power lies not only in the basic commands but also in the advanced techniques that streamline your development process. Experiment with these commands in safe environments, and soon you'll master Git, empowering you to work seamlessly in collaborative software projects. Happy coding! 🚀