# git basics [WIP]

- git is a distributed revision control system
- it consists of repos
- a repo is a directory whose contents are tracked by git
- a repo contains a set of files and their historical state
- a set of changes is captured in a commit

To start working with git, you can either create a new repo or clone an existing one.
- to clone with SSH, you need to do the following (will be described in more detail in a separate doc):
  - create an SSH key pair (public-private)
  - share the public key with the remote (e.g., github)
  - add the private key to your SSH agent for authentication

Repos can either be remote or local; local repos are on your computer.
In this case, remote repos are on github.com.

## Basic commands

### Starting git

- `git init` allows you to create a new local repo from scratch
- `git clone` lets you clone a remote repo

```
$ git clone git@github.com:arunasurya/academy.git
Cloning into 'academy'...
Warning: Permanently added the RSA host key for IP address '140.82.118.3' to the list of known hosts.
remote: Enumerating objects: 79, done.
remote: Counting objects: 100% (79/79), done.
remote: Compressing objects: 100% (78/78), done.
remote: Total 79 (delta 39), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (79/79), 21.50 KiB | 262.00 KiB/s, done.
Resolving deltas: 100% (39/39), done.
```
Now this repo is local on your computer.
- to learn of any changes made on the remote repo after cloning it, use `git fetch`
```
$ git fetch
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From github.com:arunasurya/academy
   72d79b0..7563e27  master     -> origin/master
```

- use `git merge` to merge those changes into the current branch of your local repo
```
$ git merge
Auto-merging git.md
Merge made by the 'recursive' strategy.
 git.md | 1 -
 1 file changed, 1 deletion(-)
```
- you can also use `git pull` to both fetch and merge any changes
```
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From github.com:arunasurya/academy
   da23ff9..9593959  master     -> origin/master
Updating da23ff9..9593959
Fast-forward
 git.md | 4 +---
 1 file changed, 1 insertion(+), 3 deletions(-)
```

### Branches

- each repo has at least one branch; its default branch is `master`
- you can check what branch you are on by typing `git branch`
```
$ git branch
* master
```
- to create a new branch on master, use `git checkout -b` followed by a name of the new branch

Before starting any new work, use `git status` to check the status of your repo.
- in this case, there were no changes on branch git
```

Make sure that your branch is up-to-date with the master branch on the remote repo in case you 
have made changes there that you have forgotton about or someone else has made new changes.
- you can do it in two ways
- the first way is to use `git fetch` to see all the new changes in the remote
- then then type `git merge` to merge all the new changes to your local repo
- alternatively, you can use `git pull` to fetch and merge the changes in one command

$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
```
- if there was a change in the repo, you will see the name of the modified file

- use `git diff` to see what the exact change was

- if you are happy with the changes, it is best to save them in your local repo
- use `git commit` with an argument `-am` and a simple description of the commit
- it is best to commit your changes in small chunks as it is easier to track them

- when you create a new file, you can add by using `git add`


