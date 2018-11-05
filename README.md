# BeyondHacktoberfestGT

This repository was created to explain how to make a pull request step by step. Follow the next instructions to clone the repository, create a branch, send it to GitHub, make a pull request.

## How to clone the repository

Use the following command line

```
git clone https://github.com/JDuchessGT/BeyondHacktoberfestGT.git
```

**output (can be different)**
```
Cloning into 'BeyondHacktoberfestGT'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
```

Now we need to move to the directory where the repository has been cloned using the following command line

```
cd BeyondHacktoberfestGT
```

Inside BeyondHacktoberfestGT directory use `status` command to verifying the branch

```
git status
```

**output**
```
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
```

## Creating a branch for work on it

To create a branch, use the `branch` command as shown below

```
git branch <branch-name>
```

Use a representative branch name, that reflects the action that is carried out. For example, since we are modifying this README.md file, we will use *modify-README* name, but you can use other.

```
git branch modify-README
```

To continue, we need to switch to the new branch *modify-README*, to do that we will use `checkout` command.

```
git checkout modify-README
```

**output**
```
Switched to branch 'modify-README'
```

To verify that we are in the new branch, we can use again the `status` command.

```
git status
```

**output**
```
On branch modify-README
nothing to commit, working tree clean
```

## Making our changes

For this little guide, we are only modifying this README.md file. But we can add, delete or modify other files (in the case to other repositories). To see our changes we can use the `status` command.

```
git status
```

**output**
```
On branch modify-README
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

> Note: Since we don't have our file added, _modified:   README.md_ text will be red.

## Adding our changes

We can watch in the out that we have a file modified, README.md. For can add it to our future commit and pull request we need to use the `add` command, like next:

```
git add README.md
```

**output**
```
On branch modify-README
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   README.md

```

> Note: Now that we have added the README.md file, _modified:   README.md_ text will be green.

## Creating a commit

A commit is like a revision of which changes we made over the file(s), or which file(s) we will add or remove from the branch. Commits are like a localy history, and we send all them using the `push` command to the repository. We accompany this command with `-m` to establish a message, as shown below:

```
git commit -m "Adding instructions:
• to clone a repository
• to create a branch
• to switch to the new branch"
```

**output**
```
[modify-README c2fc75f] Adding instructions: • to clone a repository • to create a branch • to switch to the new branch
 1 file changed, 119 insertions(+)
```

## Sending our changes to GitHub

As we have said, this only establishes a local history, to send our new branch and all the changes made to the repository we will use the `push` command using the following sintax.

```
git push origin <local branch name>:<repository branch name>
```

It may be good practice to use the same local name and in the repository, we will send our changes to the repository as shown below:

```
git push origin modify-README:modify-README
```

**output**
```
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 1.15 KiB | 1.15 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/JDuchessGT/BeyondHacktoberfestGT.git
   d7fff50..c2fc75f  modify-README -> modify-README
```

Since this is our first push, we can now see our branch listing in the repository.

![alt text](https://image.prntscr.com/image/rf53Id0ZSyi3LhzBzM50LA.png "Branch is now listed at the repository")

## Creating a PR (pull request) for add our changes

Since we have our branch listed in the repository, we can request the pull request from the GitHub platform, making click in the _**New pull request**_ button, that action will redirect us to the next screen.

![alt text](https://image.prntscr.com/image/xsFmLkDYT7O72QK73C3KyQ.png "Creating the PR (Pull Request)")

At this screen, we can set a new message for the pull request and finally create it making click on the _**Create pull request**_ button. Now we only have to wait for a repository administrator to approve our pull request.
