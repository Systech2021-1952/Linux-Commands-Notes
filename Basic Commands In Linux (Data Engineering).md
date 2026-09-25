# Basic Commands in Linux (Data Engineering)

**1. Present working directory:**
```bash
ubuntu@dheen:~$ pwd
/home/ubuntu
```
**2. Version:**
```bash
ubuntu@dheen:~$ uname -a
# version will appear
```
**3. Username:**
```bash
ubuntu@dheen:~$ whoami
ubuntu
```
**4. Clearing the screen:**
```bash
ubuntu@dheen:~$ clear
# Terminal will be cleared (Shortcut: Ctrl + L)
```
**5. Viewing command history:**
```bash
ubuntu@dheen:~$ history
# Total history can be viewed.
```

# Creating Directory and Files in Linux

**1. Make directory:**
```bash
ubuntu@dheen:~$ mkdir data
# Data file will be created.
```
**2. Entering into a directory:**
```bash
ubuntu@dheen:~$ cd data/
# We will be enter into 'data' file.
```
**3. Creating a text file (vi editor):**
```bash
ubuntu@dheen:~/data$ vi hello
# "hello" text file will be created.
```
* **In the editor: you have to give `i` for inserting text.
*  Enter some text.
*  Give Escape button.
* **Saving a file:** Press `Esc`, then type `:wq` to save and quit.
* **Quit without saving:** Press `Esc`, then type `:q!`

**4. List of files:**
   ```bash
   ubuntu@dheen:~/data$ ls
   hello.txt
   ```
**5. Installing a package (Linux):**
   ```bash
   ubuntu@dheen:~/data$ sudo apt-get install vim
   ```
   * `sudo`: root user privilege.
   * `apt-get`: package manager for applications.
   * `vim`: upgrading the vi editor.

 **Auto-completing a command:** 
 - Press `Tab` to auto-complete a file name.
 - (If we create two or more files)

**6. Nano Text Editor:** Simple and easy to use.
   ```bash
   ubuntu@dheen:~/data$ nano test.txt
   ```
   ```
   ubuntu@dheen:~/data$ 1s
   ```
   - Nano editor is simple, easy to use.

7. **Creating a dummy file (empty file):**
   ```bash
   ubuntu@dheen:~/data$ touch foo.txt
   ```

8. **File manipulation:**
   * **Remove (delete) a file:**
     ```bash
   1.  ubuntu@dheen:~/data$ rm foo.txt
     ```
     **List specific extension:**
     ```bash
   2.  ubuntu@dheen:~/data$ ls *.txt
     ```
     **List files starting with 'he':**
     ```bash
   3. ubuntu@dheen:~/data$ ls he*
     ```
     **Delete all files in current directory:**
     ```bash
   4.  ubuntu@dheen:~/data$ rm *
     ```
---
## 3. Viewing and Copying a File
1. **Displaying content in command prompt:**
   ```bash
   ubuntu@dheen:~/data$ cat hello.txt
   ```
2. **Copying a file (`cp`):**
   ```bash
   ubuntu@dheen:~/data$ cp hello.txt new-hello.txt
   ```
3. **Renaming a file (`mv`):**
   ```bash
   ubuntu@dheen:~/data$ mv hello.txt demo.txt
   ```
4. **Copying a file with `cat` command (Append `>>`):**
   ```bash
   ubuntu@dheen:~/data$ cat demo.txt >> nfile.txt
   ```















