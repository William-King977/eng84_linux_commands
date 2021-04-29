# Linux Commands Interview Questions
* **How to check Hidden Files and Directories?**
  * `ls -a` - lists all hidden files and directories in the current directory

* **What are Flags?**
  * Flags are a way to set options and pass in arguments to the commands you run. These will change the behaviour of the commands.
  * E.g. running `ls` with the `-l` flag will show more information and change the output format. 

* **What is a Wildcard and how do you use them?**
  * A symbol or a set of symbols that represent other characters.
  * `*` - any number of characters. E.g. `ls p*` lists files starting with `p`.
  * `?` - single occurrence of any character. E.g. `ls l?st.txt` lists files starting with `l` and ending with `st.txt`.
  * `[]` - matches any occurrence of a character in the brackets. E.g. `ls [abdcio]ist.txt` lists files starting with one of the characters inside the brackets and ends with `ist.txt` (`cist.txt`, `dist.txt` etc.).

* **How can you do Process Management?**
  * Controlling the current processes in the foreground and background. Some commands are shown below and the next two questions.
  * `sudo systemctl` - controls a single process with `status`, `start`, `stop` or `restart`. E.g. `systemctl status nginx` checks if nginx is running.

* **What is Currently Running on your system?**
  * `top` - displays all current foreground and background processes in real-time
  * `ps` - displays all current foreground processes at that point
  * `ps aux` - similar to `top`, but not in real-time

* **Checking and stopping/killing processes running in the foreground and background**
  * Using `top` - While this is showing, one can press `k` to kill a process and is prompt to enter its `PID` (process ID)
  * `kill PID` - stop a process based on its `PID` (outside of `top`)

* **How to change permissions with the `chmod` command?**
  * `chmod +w filename` - grants write permission to the file
  * `chmod -wx filename` - revokes write and execute permissions from the file
  * Can be applied to the user (`u`), a group (`g`), others (`o`) or all (`a`)
  * `chmod u=+w filename` grants write permission to the user, but revokes previously granted permissions 

* **What does `777`, `400`, `600`, `r`, `w`, `x` mean?**
  * `777` - read, write and execute permission for any user
  * `400` - grants read permission to the user only
  * `600` - grants read and write permissions to the user only
  * `r` - read permission
  * `w` - write permission
  * `x` - execute (file) permission

* **How to check permission for files/dir?**
  * `ll` - checks permissions for every file/dir in the current directory
  * `ll directory` - checks permissions for every file/dir in the specified directory
  * `ll filename` - checks permissions for the specified file
  * `ls -ld` - checks permissions for the current directory
  * `ls -ld directory` - checks permissions for the specified directory
  * `ls -l` does the same thing as `ll`

* **How to use `head`, `tail`, `sort`, `nl` (number line) and `wc` (word count)?**
  * `head` - prints the first 10 lines of a file
  * `tail` - prints the last 10 lines of a file
  * `sort` - sorts the file's contents, but the file is not modified
  * `nl` - prints a file with numbered lines
  * `wc` - prints number of lines, words and characters in a file (`lines words characters filename`)
  * The above commands can be used like this: `head filename`

* **What is pipping and redirection?**
  * `|` - passes the output from one command to another (to use as input). E.g. `sort file.txt | head` will sort the file, then display the first 10 lines of the sorted file. Any number of commands can be piped.
  * `>` - saves content to a file and if the file exists, it overwrites the existing contents. E.g. `file1.txt > file2.txt`.
  * `>>` - appends content to the end of a file. E.g. `file1.txt >> file2.txt`.

* **What is Standard Input and Output?**
  * `stdin` - Standard input. Takes text as input.
  * `stdout` - Standard output. Output of a command is stored in the stdout stream and is shown on the shell.
