# Linux Commands Interview Questions
* How to check Hidden Files and Directories?
  * `ls -a` - lists all hidden files and directories in the current directory

* The Manual, Flags

* What is a Wildcard and how do you use them?

* How can you do Process Management?

* What is Currently Running on your system?

* Killing a processes/crashed process

* How to check any process running in foreground and background jobs?

* How to stop/kill any process running in foreground and background jobs?

* How to change permissions with the `chmod` command?
  * `chmod +w filename` - grants write permission to the file
  * `chmod -wx filename` - revokes write and execute permissions from the file
  * Can be applied to the user (`u`), a group (`g`), others (`o`) or all (`a`)
  * `chmod u=+w filename` grants write permission, but revokes previously granted permissions 

* What does `777`, `400`, `600`, `r`, `w`, `x` mean?
  * `777` - read, write and execute permission for any user
  * `400` - grants read permission to the user only
  * `600` - grants read and write permissions to the user only
  * `r` - read permission
  * `w` - write permission
  * `x` - execute (file) permission

* How to check permission for files/dir?
  * `ll` - checks permissions for every file/dir in the current directory
  * `ll directory` - checks permissions for every file/dir in the specified directory
  * `ll filename` - checks permissions for the specified file
  * `ls -ld` - checks permissions for the current directory
  * `ls -ld directory` - checks permissions for the specified directory
  * `ls -l` does the same thing as `ll`

* How to use `head`, `tail`, `sort`, `nl` (number line) and `wc` (word count)?
  * `head` - prints the first 10 lines of a file
  * `tail` - prints the last 10 lines of a file
  * `sort` - sorts the file's contents, but the file is not modified
  * `nl` - prints a file with numbered lines
  * `wc` - prints number of lines, words and characters in a file (`lines words characters filename`)
  * The above commands can be used like this: `head filename`

* What is pipping and redirection?
  * `|`
  * `>`
  * `>>`

* What is Standard Input and Output?
  * `stdin` -
  * `stdout` -
