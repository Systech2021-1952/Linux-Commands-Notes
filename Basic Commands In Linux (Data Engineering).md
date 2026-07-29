# Basic Commands In Linux

### (1) Present working directory:

`ubuntu@dheen:~\$ pwd`

= /home/upuntu

### (2) Version:

`ubuntu@dheen:~\$ uname -a`

= version will appear

 ### (3) Username:
  
`ubuntu@dheen:~\$ whoami`

= ubuntu

### (4) Clearing the screen:
  
`ubuntu@dheen:~\$ clear` (ctrl +L)

= Terminal will be cleared.

### (5) Viewing command history:

`ubuntu@dheen:~\$ history`

= Total history can be viewed.

----------

## Creating Directory and Files in Linux

(1) Make directory:

ubuntu@dheen:~\$ mkdir data

- = Data file will be created.

- (2) Entering into a directory:

- = We will be enter into ‘data’ file.

- € Creating a text file:

- = “hello” text file will be created.

## Text file creation

- = In the editor, you have to give “i” for inserting a text.

- = Enter some text.

- = Give Escape button.

- = Forsavingafile = :wq — save

- (4) List of files:

ubuntu@dheen:~/data\$ 1s

= hello.txt.


## (5) Quit file without saving:

- In the editor — give Escape.

## Installing a package: (Linux)

ubuntu@dheen:~/data\$ sudo apt-get install vim

sudo = root user

apt-get = getting any application

vim = upgrading vi editor

## Auto-completing a command:

- Press Tab for auto-complete a file.

- (If we create two or more files).

## In data directory:


## (6) Nano Text Editor:

ubuntu@dheen:~/data\$ nano test.txt

ubuntu@dheen:~/data\$ ls

= Htest.py hello.txt hellol hello.ho test.txt

- Nano editor is simple, easy to use.

## (7) Creating a dummy file:

ubuntu@dheen:~/data\$ touch foo.txt

(After Is)

hello.txt hellol

= Htest.py

foo.txt test.txt

## (8) File manipulation: ®

- remove (deleting) a file: v/

ubuntu@dheen:~/data\$ rm foo.txt

(After Is)

= Htest.py hello.txt hellol test.txt

ubuntu@dheen:~/data\$ 1s *.txt

= hello.txt test.txt

ubuntu@dheen:~/data\$ ls he*

= hello.txt hellol

ubuntu@dheen:~/data\$ rm *

= Total files be deleted.
