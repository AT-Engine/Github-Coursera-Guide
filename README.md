# Git Branches Guide

Welcome back! In this task, we'll dive into branches in Git. If you're wondering, "What's a branch?" -- you're in the right place. Let's get started.

Think of a project's repository as the trunk, where production-ready code resides, ready to be released into the world. But what if you need to make changes, additions, or deletions? You do that in a safe space, which is where branches come in. A branch is a copy of the trunk's code where you can work safely, like a sandbox.

## Checking Current Branch

To begin, let's check which branch we're currently working in. Type `git branch` to see. By default, we're often in the master branch, which is the trunk. Any branches we create off master can be integrated back into it later.

## Creating and Switching Branches

Now, let's create a development branch named `rhyme-init`. Use `git branch rhyme-init` to create it, then `git checkout rhyme-init` to switch to it. This way, our work in `rhyme-init` won't affect the master branch.

## Creating and Switching to a New Branch

If we decide we need another branch, like `rhyme2`, we can create and switch to it simultaneously with `git checkout -b rhyme2`. Keep in mind, `rhyme2` will be based on the current branch (`rhyme-init` in this case), carrying over any changes made in `rhyme-init`.

## Making Changes and Committing

Now, let's modify a file, say `helloworld.c`, and add a comment. Save the file and use `git status` to see the changes. Stage the file with `git add helloworld.c`, then commit the changes using `git commit -m "Adding a comment"`.

## Setting Upstream and Pushing Changes

Since we forked the original repo into our account, we need to set the upstream repository. Use `git remote add upstream <repo-url>` to define the upstream repository. This connection ensures GitHub knows where to push our changes.

## Creating a Pull Request

Finally, push the changes to GitHub using `git push origin <branch-name>`. This command will also provide a link to create a pull request. Follow the provided link, fill out the pull request form with the necessary details, and click "Create pull request."

And that's it! You've completed your first commit, push, and pull request in a Git repository. In the next task, we'll explore how to keep our local repository up to date.
