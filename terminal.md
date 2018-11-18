## Terminal basics

### What is a terminal?

- computer program
- allows you to interact with the computer via text
- you provide inputs and receive outputs

### If you have a mac, how can you start a terminal?

- start the Terminal app (go to spotlight and type "terminal") 
- pre-installed on every mac
- you will see some text that ends with a `$` sign
- you can type your commands there

### Useful commands

- `whoami` command shows the name of the current user
```
$ whoami
aruna
```
- `pwd` shows the directory you are currently in (present working directory)
```
$ pwd
/Users/aruna
```
- `ls` shows the files in the current directory
```
$ ls
Desktop  Documents  Downloads  Library	Movies	Music  Pictures  Public  src
```
- `cd` lets you switch to a new directory (change directory) 
```
$ cd src
$ ls
github.com
$ cd github.com/
$ ls
arunasurya  bitcoin
$ pwd
/Users/aruna/src/github.com
```

### File vs. directory

- All files in a family of operating systems such as UNIX are in a tree like structure

`mkdir` creates a directory
```
$ mkdir test
$ ls
arunasurya  bitcoin  test
```

