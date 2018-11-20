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

- each command has one standard input (STDIN), one standard output (STDOUT) and one standard error (STDERR)

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

- all files and directories in systems such as UNIX are in a tree like structure
- there is no fundamental difference between a file and a directory
- there is some metadata that tells the operating system if something is a file or a directory

`mkdir` creates a directory
- anything that follows a command and is separated by space is an argument
- `test` is the only argument of 'mkdir` in the example below
```
$ mkdir test
$ mkdir test/happy
$ ls test/
happy
```
`touch` command creates a file
```
$ touch test/testy
$ ls test
happy  testy
```
- to check if something is a file or a directory, type `file`
- 'file' will also tell you if a file is empty or not
```
$ file test/happy
test/happy: directory
$ file test/testy
test/testy: empty 
```
`tree` command allows you to see a subtree of the current directory
```
$ tree 
.
├── happy
├── test.test
│   └── chipmunk
└── testy

3 directories, 1 file
```
`echo` command echoes arguments into its standard output
```
$ echo hello
hello
```
- to write simple messages into a file, you can use `echo` and redirect its standard output into a file (such as testy)
- use the `cat` command to see what is inside the file
```
$ echo hello aruna > testy
$ cat testy
hello aruna
```
Using `echo` in this way will replace the contents of the file. If you want to append text to the file, you can use it like this:
```
$ echo howdy! >> testy
$ cat testy
hello aruna
howdy!
```


