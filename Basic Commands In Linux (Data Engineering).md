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
```
**2. Entering into a directory:**
```bash
ubuntu@dheen:~$ cd data/
```
**3. Creating a text file (vi editor):**
```bash
ubuntu@dheen:~/data$ vi hello
```
* **Text file creation steps:**
  * Press `i` to insert text.
  * Enter your text.
  * Press `Esc` to exit insert mode.
  * For saving and quitting: `:wq`
  * Quit without saving: `:q!`
**3. Creating a text file (vi editor):**
```bash
ubuntu@dheen:~/data$ vi hello
```
* **Text file creation steps:**
  * Press `i` to insert text.
  * Enter your text.
  * Press `Esc` to exit insert mode.
  * For saving and quitting: `:wq`
  * Quit without saving: `:q!`
**5. Installing a package:**
```bash
ubuntu@dheen:~/data$ sudo apt-get install vim
# sudo: root user
# apt-get: getting any application
# vim: upgrading vi editor
```




























