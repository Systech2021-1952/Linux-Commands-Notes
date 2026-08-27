# Basic Commands in Linux


### 1. Present working directory:
ubuntu@root:~$ pwd
> /home/ubuntu

### 2. Version:
ubuntu@root:~$ uname -а
> version will appear

### 3. Username:
ubuntu@root:~$ whoami 
> ubuntu

### 4. Clearing the screen:
ubuntu@root:~$ clear          (ctrl + l)
> Terminal will be cleared.

### 5. Viewing command history:
ubuntu@root:~$ history
> Total history can be viewed.

- ## Creating Directory and Files in Linux

### 1. Make directory:
ubuntu@root:~$ mkdir data
> Data file will be created.

### 2. Entering into a directory:
ubuntu@root:~$ cd data/
> We will be enter into 'data' file.

### 3. Creating a text file:
ubuntu@root:~/data$ vi hello
> "hello" text file will be created.

- ### Text file creation
- In the editor, you have to give "¡" for inserting a text.
- Enter some text.
- Give Escape button.
- For saving a file ` wq : → save `
- Without saving a file ` :b → quit `

### 4. List of files:
ubuntu@root:~/data$ 1s
> hello.txt.

### 5. Quit file without saving:
- In the editor → give Escape.
  
` :q! `

 ## Installing a package: (Linux)
ubuntu@root:~/data$ sudo apt-get install vim

`sudo` root user

` apt-get`getting any application

` vim ` upgrading vi editor

### Auto-completing a command:

- Press Tab for auto-complete a file.

(If we create two or more files).


## In data directory:
`   hello.txt   hello1   hello.py    `

- If we give ⇒ vi hello
  
  output ⇒ hello.txt hello1 hello.py

- If we give ⇒ viP hello

  output ⇒ hello.txt hello.py

- If we give ⇒ VP hello
 
  output ⇒ hello.txt hello.py


## 6. Nano Text Editor:
```
ubuntu@root:~/data$ nano test.txt
```
```
ubuntu@root:~/data$ 1s 
```
⇒ Htest.py hello.txt hello1 hello.ho test.txt

> Nano editor is simple, easy to use.

##  7. Creating a dummy file:

```
ubuntu@root:~/data$ touch foo.txt
```
(After Is)

⇒ Htest.py hello.txt hello1 foo.txt test.txt

## 8. File manipulation:

- ### remove (deleting) a file:

```
1. ubuntu@root:~/data$ rm foo.txt
```

(After Is)

⇒ Htest.pу hello.txt hello1 test.txt

```
2. ubuntu@root:~/data$ 1s *.txt
```
⇒ hello.txt test.txt
```
3. ubuntu@root:~/data$ ls he*
```
⇒ hello.txt hello1
```
4. ubuntu@root:~/data$ rm *
```
⇒ Total files be deleted.

# Viewing and Copying a File
```
ubuntu@root:~/data$ vi hello.txt
```
(hello.txt will some text is created).
### 1. Displaying content in command prompt:
` ubuntu@root:~/data$ cat hello.txt ` // cat

⇒ This is a file that is created.

### 2. Copying a file: (X)
` ~/data$ cp hello.txt new-hello.txt ` // cp

` ~/data$ 1s `
⇒ hello.txt      new-hello.txt

### 3. Renaming a file:
` ~/data$ mv hello.txt demo.txt ` // mv

` ~/data$ 1s `

⇒ demo.txt    new-hello.txt

` ~/data$ cat demo.txt `

⇒ This is a file that is created.

### 4. Copying a file with 'cat' command:

` Append symbol (>>): `

`
ubuntu@root:~/data$ cat demo.txt >> nfile.txt
`

(After ls)

⇒ demo.txt    new-hello.txt    nfile.txt

(Copies the text from one file to another).

### 5. Printing texts in prompt:
1. `~/data$ echo "root" ` // echo

⇒ root

2. ` ~/data$ echo "dheen" >> nfile.txt ` // store in file

(The text will be stored in file).

3. ` ~/data$ echo "mohamed" >> nfile.txt `  // append in file

   ` ~/data$ cat nfile.txt `

  ⇒ This is a file that is created

  dheen

  mohamed

# File Navigation System 
### 1. ls and cd commands:
` ubuntu@root:~$ 1s `

⇒ untitled.pnb data print_time.py

   airflow data.log retal.txt
   
---

### Shortcut for "home/ubuntu":
` ubuntu@root:~$ cd data/ `

` ubuntu@root:~/data$ data.log `

- No such file directory
  
:~/data $ cd.         N→ Home directory

:~$ vi data.log      →cd ~ 

Give "This is a log file" and save it.

⇒:~$ cd data/

:~/data $ cd..

:~$ cd data

(home/ubuntu/data. log)

"This is a log file"

```
* → :~/data~ /data.log  (/~)
"This is a log file".
```

### 2. Creating nested Directory:

- If we want to create directory (or) file in the file that doesn't exist (or) created
- we have to create it one by one into a file.
- Instead we use "-p".

` ubuntu@root:~$ pwd `   /* //-p
/home/ubuntu

` ubuntu@root:~$ mkdir -p abc/test/demo `

~$ cd abc/
~$1s

⇒ test

### 3. Going Back from a directory:

` ubuntu@root:~$ cd abc/test/demo `

` ubuntu@root:~$ pwd `

/home/ubuntu/abc/test/demo

ubuntu@root:~$ cd ..   (home/ubuntu/abc/test)

ubuntu@root:~$ cd../..   (home/ubuntu)

ubuntu@root:~$ cd -      (will go to previous cd command)

/home/ubuntu/abc/test

### 5. Printing texts in prompt:

1. data$ echo "dheen" // echo
⇒ dheen








