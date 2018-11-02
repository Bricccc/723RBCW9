# 723RBCW9
This is the BASH HW by Brita

So this is the course *From Newbies for Newbies: BASH* 
## BASH! WHY BASH?
So to answer to this question I have gathered some information and created a small video on Youtube:

<iframe width="560" height="315" src="https://www.youtube.com/embed/UwA90p9GzGU" ></iframe>


## BASH! FILES AND DIRECTORIES
Files and Directories are slightly looked at in this video:

<iframe width="560" height="315" src="https://www.youtube.com/embed/qw-JPsR6_aQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The scenario for this demo is to show how to create directories and files (basic txt files) and to show how to navigate through these directories and something more.  

```sh
$ whoami
root
$ tree
.

0 directories, 0 files
$ mkdir First
$ ls -la
total 3
drwxr-xr-x  3 root root  4 Nov  2 16:45 .
drwx------ 10 root root 16 Nov  2 15:28 ..
-rw-------  1 root root 42 Nov  2 16:45 .bash_history
drwxr-xr-x  2 root root  2 Nov  2 16:45 First
$ tree
.
└── First

1 directory, 0 files
$ cd First
$ mkdir -p Second/Third/Brita
$ tree
.
└── Second
    └── Third
        └── Brita

3 directories, 0 files
$ cd ..
$ pwd
/root/sandbox
$ tree
.
└── First
    └── Second
        └── Third
            └── Brita

4 directories, 0 files
$ cd First/Second/Third
$ echo "Tekstinjsh" > Teksts.txt
$ can Teksts.txt
bash: can: command not found
$ ls -la
total 2
drwxr-xr-x 3 root root  4 Nov  2 16:47 .
drwxr-xr-x 3 root root  3 Nov  2 16:46 ..
drwxr-xr-x 2 root root  2 Nov  2 16:46 Brita
-rw-r--r-- 1 root root 11 Nov  2 16:47 Teksts.txt
$ man cat
$ cat Teksts.txt
Tekstinjsh
$ echo "I append this row to my file" >> Teksts.txt
$ cat Teksts.txt
Tekstinjsh
I append this row to my file
$ tree
.
├── Brita
└── Teksts.txt

1 directory, 1 file
$ cd ..
$ touch "another text" Teksts2.txt
$ cd ..
$ cd ..
$ cd ..
$ tree
.
└── sandbox
    └── First
        └── Second
            ├── Teksts2.txt
            ├── Third
            │   ├── Brita
            │   └── Teksts.txt
            └── another text

5 directories, 3 files
$ pwd
/root
$ cd sandbox
$ pwd
/root/sandbox
$ cd First/Second
$ pwd
/root/sandbox/First/Second
$ mv Teksts2.txt Third
$ pwd
/root/sandbox/First/Second
$ cd Third
$ ls -la
total 3
drwxr-xr-x 3 root root  5 Nov  2 16:53 .
drwxr-xr-x 3 root root  4 Nov  2 16:53 ..
drwxr-xr-x 2 root root  2 Nov  2 16:46 Brita
-rw-r--r-- 1 root root 40 Nov  2 16:49 Teksts.txt
-rw-r--r-- 1 root root  0 Nov  2 16:49 Teksts2.txt
```



## BASH! EDITING (?)
Not quite sure about this yet :)

https://bricccc.github.io/723RBCW9/

