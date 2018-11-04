# BeyondHacktoberfestGT

Repository created for test a PullRequest

## How to clone the repository

Use the following command line

```
git clone https://github.com/JDuchessGT/BeyondHacktoberfestGT.git
```

**A posible output**

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

Now inside BeyondHacktoberfestGT directory use `git status` command line to verifying the branch

```
git status
```

**output***

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

**output***

```
Switched to branch 'modify-README'
```

To verify that we are in the new branch, we can use again the `status` command.

```
git status
```

**output***

```
On branch modify-README
nothing to commit, working tree clean
```

## Making our changes

For this little guide, we are only modifying this README.md file. To see our changes we can use the status command.

```
git status
```

**output***

```
On branch modify-README
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```

```
git add README.md
```

**output***

```
On branch modify-README
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   README.md

```

## Creating a PR (pull request) for add our changes

