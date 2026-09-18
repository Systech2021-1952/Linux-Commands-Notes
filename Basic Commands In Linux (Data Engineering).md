# Basic Commands in Linux (Data Engineering)
## 1. Basic Commands in Linux
1. **Present working directory:**
   ```bash
   ubuntu@dheen:~$ pwd
   /home/ubuntu
   ```
2. **Version:**
   ```bash
   ubuntu@dheen:~$ uname -a
   ```
3. **Username:**
   ```bash
   ubuntu@dheen:~$ whoami
   ubuntu
   ```
4. **Clearing the screen:**
   ```bash
   ubuntu@dheen:~$ clear
   # Or use shortcut: (ctrl + L)
   ```
5. **Viewing command history:**
   ```bash
   ubuntu@dheen:~$ history
   ```

---

## 2. Creating Directory and Files in Linux
1. **Make directory:**
   ```bash
   ubuntu@dheen:~$ mkdir data
   ```

2. **Entering into a directory:**
   ```bash
   ubuntu@dheen:~$ cd data/
   ```

3. **Creating a text file (using `vi` editor):**
   ```bash
   ubuntu@dheen:~/data$ vi hello
   ```
   * **In the editor:** Press `i` for inserting text.
   * **Saving a file:** Press `Esc`, then type `:wq` to save and quit.
   * **Quit without saving:** Press `Esc`, then type `:q!`

4. **List of files:**
   ```bash
   ubuntu@dheen:~/data$ ls
   hello.txt
   ```
   
5. **Installing a package (Linux):**
   ```bash
   ubuntu@dheen:~/data$ sudo apt-get install vim
   ```

   * `sudo`: root user privilege.
   * `apt-get`: package manager for applications.
   * `vim`: upgrading the vi editor.

   **Auto-completing a command:** 
     - Press `Tab` to auto-complete a file name.
     - (If we create two or more files).

6. **Nano Text Editor:** Simple and easy to use.
   
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

    (After Is)

    `test.py`  `hello.txt`  `hello1`  `foo.txt`   `test.txt`

8. **File manipulation:**
   
   * **Remove (delete) a file:**

   ```bash
   1.  ubuntu@dheen:~/data$ rm foo.txt
   ```
    (After Is)

    ` Htest.pу ` ` hello.txt ` ` hello1 `  ` test.txt `

   ```bash
   2.  ubuntu@dheen:~/data$ ls *.txt
   ```
    `hello.txt`  `test.txt`

   ```bash
   3. ubuntu@dheen:~/data$ ls he*
   ```
   `hello.txt`  `hello1`
   
   ```bash
   4.  ubuntu@dheen:~/data$ rm *
   ```
   . Total files be deleted.

##  3. Viewing and Copying a File

 ```
 ubuntu@dheen:~/data$ vi hello.txt
 ```

 (hello.txt will some text is created).



1. **Displaying content in command prompt:**
   
    ` ubuntu@dheen:~/data$ cat hello.txt ` //cat
  
   
2. **Copying a file (`cp`):**
   
    ` ubuntu@dheen:~/data$ cp hello.txt new-hello.txt `  // cp
  
    ` ~/data$ 1s ` 
   
3. **Renaming a file (`mv`):**
   
   ` ubuntu@dheen:~/data$ mv hello.txt demo.txt `

   ` ~/data$ 1s `
   
4. **Copying a file with `cat` command :**

   ` (Append `>>`): `
   
   ` ubuntu@dheen:~/data$ cat demo.txt >> nfile.txt `

   (After ls)

   ` demo.txt `  ` new-hello.txt `  ` nfile.txt `
      
   (Copies the text from one file to another).
   
5. **Printing texts in prompt (`echo`):**
   
   ubuntu@dheen:~/data$ echo "dheen"
   
   * **Store in file:** `echo "dheen" >> nfile.txt` (Appends text to the file)

---












