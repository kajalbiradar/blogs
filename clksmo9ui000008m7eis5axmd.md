---
title: "📚 Advanced Git and GitHub🚀"
datePublished: Tue Aug 01 2023 18:23:49 GMT+0000 (Coordinated Universal Time)
cuid: clksmo9ui000008m7eis5axmd
slug: advanced-git-and-github
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1690913940840/ca3bcf23-ed4c-4b7d-a128-b7b6643fcdb0.png
tags: github, git, devops, 90daysofdevops, trainwithshubham

---

## Introduction

Welcome to this comprehensive guide on Git, the powerhouse of version control in the world of software development! Git empowers developers to work collaboratively, efficiently manage code changes, and ensure seamless teamwork. In this blog, we'll explore advanced Git concepts such as branching, reverting, resetting, rebasing, and merging. These essential features play a crucial role in maintaining a clean codebase and facilitating efficient development workflows. So, let's embark on this journey to master the art of Git! 🌟

## Git Branching: Navigating through Parallel Universes 🌳

Branching in Git is akin to creating parallel universes within your project. Each branch represents a unique development path, allowing developers to work on features or bug fixes in isolation. In this section, we'll cover the following key aspects:

* Creating branches: Learn how to create new branches to tackle different tasks and features concurrently.
    
* Switching branches: Master the art of seamlessly switching between branches, enabling you to focus on specific development tasks.
    
* Merging branches: Explore the process of integrating changes from one branch into another, promoting collaboration and code harmonization.
    

```bash
# Create a new branch 'feature-login' and switch to it
git checkout -b feature-login

# Make changes to the code
# (Make sure to create, modify, or delete files related to the 'login' feature)

# Commit your changes with a descriptive message
git add .
git commit -m "Implement login feature"

# Switch back to the 'master' branch
git checkout master
```

## Git Revert and Reset: Rewinding Time in Your Repository ⏪

Sometimes, mistakes happen, or changes prove to be problematic. Git offers two essential mechanisms to undo previous changes: revert and reset. Let's explore these options:

* Reverting commits: Safely undo changes without altering the commit history, ensuring a clean track record of actions taken.
    
* Resetting commits: Move the branch pointer to an earlier commit, effectively "rewinding" the repository's state.
    

```bash
# Revert a specific commit (creates a new commit to undo changes)
git log

# Copy the commit ID you want to revert
git revert <commit_id>

# Reset to a previous commit (be cautious as it discards commits after the specified commit)
git log

# Copy the commit ID you want to reset to
git reset --hard <commit_id>
```

## Git Rebase and Merge: Rewriting History and Harmonizing Code 🔄

Rebase and merge are vital techniques for integrating changes from one branch into another. Each method has its advantages and use cases:

* Git Rebase: Rework the commit history to create a cleaner and more linear sequence, simplifying the development process.
    
* Git Merge: Merge changes into the target branch as a new commit, preserving the original commit history.
    

```bash
# Git Rebase: Apply changes from 'feature-login' onto 'master'
git checkout feature-login
git rebase master

# Git Merge: Merge 'feature-login' into 'master' with a commit message
git checkout master
git merge feature-login -m "Merge feature-login into master"
```

## Best Practices for Effective Git Workflow 🏆

To maintain a robust and efficient Git workflow, consider the following best practices:

* Feature branch workflow: Organize development tasks using separate feature branches for each new functionality.
    
* Keeping a clean commit history: Write clear, descriptive commit messages and squash related commits before merging.
    
* Collaboration and code review: Foster collaboration through pull requests and code reviews, ensuring high-quality code contributions.
    

```bash
# Feature branch workflow
git checkout -b feature-new-functionality
# Work on the new functionality
git add .
git commit -m "Implement new functionality"
# Request code review and merge into 'master' when ready

# Squash related commits before merging
git log
git rebase -i HEAD~n
# In the interactive rebase, 'pick' the oldest commit and 'squash' the rest
```

## Task:

🌟 Welcome to this exciting task where we'll delve into the world of Git and explore creating a new branch, making changes with various commit messages, and reverting a file to an earlier version. Let's follow these simple steps to master these powerful Git features! 🚀

Step 1: Create a New Branch 🌿

First, navigate to the "d:/day10" directory in your local repository and intialize it:

```bash
cd d:/day10
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690912362259/f3c14d5c-0550-437a-bb08-f816fc7bfe84.png align="center")

Next, create a new branch called "dev" that will branch off from the "master" branch:

```bash
git checkout -b dev
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690912422463/2997b05f-fa18-478e-b238-2b381574cd6f.png align="center")

Congratulations! You've now created and switched to the "dev" branch. Any changes you make will be isolated from the "master" branch until you decide to merge them.

Step 2: Make Changes with Various Commit Messages 📝

```plaintext
This is the first feature of our application.
```

Now, let's commit this change with a descriptive message:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690912562276/f35eb4c6-ba98-493f-8c59-d095f4d012e1.png align="center")

Great! You've made your first commit in the "dev" branch with the message "Added the first feature."

Let's continue making more changes to the "version01.txt" file:

```plaintext
This is the bug fix in development branch.
```

Now, commit this change with another informative message:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690912691242/68ad1b1e-97de-4ac4-8ff5-750f53bad9f3.png align="center")

Fantastic! You've added a second commit with the message "Fixed a bug in development branch."

Now, add more content to the file in similar way:

```plaintext
This is some new feature in development branch.
```

```plaintext
This is gadbad code
```

```plaintext
This feature will gadbad everything from now.
```

Step 3: Reset a File ⏪

We can use `git reset` to move the "dev" branch pointer back to the commit before the bug fix:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690913109838/5ae6cf10-ac5a-49ba-8081-70cf6ec52150.png align="center")

```bash
git reset --hard <commit_id>
```

Caution: When using `git reset --hard`, all changes after the specified commit will be permanently discarded, so be sure to back up any important changes.

You've successfully completed the tasks of creating a new branch, making changes with various commit messages, and restoring a file to an earlier version using Git. Keep exploring and mastering these Git features to become an exceptional developer! 🎉🌟

## Conclusion:

Congratulations! You've completed this comprehensive guide on mastering Git's advanced features. From branching and merging to reverting and rebasing, you now possess a powerful toolkit to handle complex development tasks with ease. Remember, practice is key to becoming a proficient Git user. So, keep exploring, experimenting, and refining your skills to unlock the full potential of Git in your software development journey! 🚀🌟