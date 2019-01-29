# git basics

- git is a distributed revision control system
- consists of repos
- a repo is a directory whose contents are tracked by git
- it contains a set of files and their historical state
- a set of changes is captured in a commit

To start working with git, you can either create a new repo or clone an existing one.
- to clone with SSH, you need to do the following:
  - create an SSH key pair (public-private)
  - share the public key with the remote (e.g., github)
  - add the private key to your SSH agent for authentication

Repos can either be remote or local; local repos are on your computer.
In this case, remote repos are on github.com.

## Basic commands

`git init` allows you to create a new local repo from scratch

`git clone` lets you clone a remote repo

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
- now this repo is local on your computer
- to learn of any changes made on the remote repo after cloning it, use `git fetch` 

- each repo has at least one branch; its default branch is `master`
- you can check what branch you are on by typing 'git branch'

```
$ git branch
* master
```

- before starting any new work, use `git status` to check the status of your repo
- in this case, there were no changes on branch git
```
$ git status
On branch git
nothing to commit, working tree clean
```
- if there was a change in the repo, you will see the name of the modified file
```
$ git status
On branch git
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   git.md

no changes added to commit (use "git add" and/or "git commit -a"
```
- use `git diff` to see what the exact change was

- if you are happy with the changes, it is best to save them in your local repo
- use `git commit` with an argument `-am` and a simple decription of the commit
