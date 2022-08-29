# UNIX Commands

* Commands
  * [`bash`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#bash)
  * [`cat`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#cat)
  * [`cd`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#cd)
  * [`cp`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#cp)
  * [`chgrp`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#chgrp)
  * [`chmod`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#chmod)
  * [`chown`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#chown)
  * [`chsh`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#chsh)
  * [`csh`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#csh)
  * [`dash`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#dash)
  * [`diff`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#diff)
  * [`env`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#env)
  * [`find`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#find)
  <!-- * [`fs`]() -->
  * [`grep`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#grep)
  * [`head/tail`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#headtail)
  * [`history`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#history)
  * [`jobs, fg, bg`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#jobs-fg-bg)
  * [`kill`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#kill)
  * [`last`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#last)
  * [`less`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#less)
  * [`ln`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#ln)
  * [`locate/updatedb`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#locateupdatedb)
  * [`ls`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#ls)
  * [`man`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#man)
  * [`mkdir`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#mkdir)
  * [`more`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#more)
  * [`mv`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#mv)
  * [`printenv`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#printenv)
  * [`ps`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#ps)
  * [`ps aux`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#ps-aux)
  * [`ps elf`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#ps-elf)
  * [`pwd`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#pwd)
  * [`rm`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#rm)
  * [`rmdir`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#rmdir)
  * [`set`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#set)
  * [`sh`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#sh)
  * [`sort`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#sort)
  * [`strings`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#strings)
  * [`su`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#su)
  * [`sudo`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#sudo)
  * [`touch`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#touch)
  * [`uniq`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#uniq)
  * [`wc`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#wc)
  * [`which`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#which)
  * [`zsh`](https://github.com/akk20/HPU-System-Security/tree/main/UNIX%20Commands#zsh)
* Command Line Metacharacters
  * `|` pipe
  * `>` output redirection
  * `<` input redirection
  * `*` and `?` wild cards in the identification of files
  * `$` - used in matching patterns – matches end of line
  * `^` - similar to `$` but matches the beginning of line
  * `~` home directory

## Commands

### `bash`

### `cat`
Print contents of file in the command window

```bash
cat <file>
```
---
### `cd`
Change directories

```bash
cd <directory>
```
---
### `cp`
Copy the contents of `file` into `file2`

```bash
cp <file> <file2> 
```
---
### `chgrp`
### `chmod`
Change the permission of any file

```bash
chmod <permissions> <file>
```
Permissions
* A three digit number to represent the permisson for `user-group-world`
* `rwx`
  * `r` has permisson to read the file
  * `w` has permisson to write to the file
  * `x` has permisson to execute the file
  * `---` means no permissions have been granted at all
* How to calulate command
  * For each `rwx` in the user, group, and world, put a `1` to allow or `0` to deny a specific permisson.
  * Ex: `111` `101` `100` mean the file can be:
    * read, written and executed by the user
    * read, **not** written, and executed by the group
    * read, **not** written, and **not** executed by the world
  * To put this on the command line, each of the three section need to be converted from binary to decimal
    * `111` would equal `7`
    * `101` would equal `5`
    * `100` would equal `4`
  * So the final command for this example would be `chmod 754 <filename>`
---
### `chown`
### `chsh`
### `csh`
### `dash`
### `diff`
### `env`
### `find`
<!-- ### `fs`


```
fs
```
--- -->
### `grep`
`grep` is the **g**eneralized **r**egular **e**xpression **p**arser.


`gerp "pattern" <filename>` This command displays all the lines in the filename which contains the pattern "pattern" (case sensitive).

`gerp -i "pattern" <filename>` This command displays all the lines in the filename which contains the pattern "pattern" (case insensitive).

`gerp -c "pattern" <filename>` This command displays the count of the lines having the pattern "pattern"

`gerp -v "pattern" <filename>` This command displays the lines of the file which does not have the pattern "pattern".

`gerp -l "pattern" *` This command displays the filenames in the current directory which has the pattern "pattern".

---
### `head`/`tail`
`head <filename>` will display the first lines in the listed files, by default it displays first 10 lines of the file.
`head -25 <filename>` will display the first 25 lines in the listed files.

`tail <filename>` will display the last lines in the listed files, by default it displays first 10 lines of the file.
`tail -25 <filename>` will display the last 25 lines in the listed files.
### `history`
List history of all commands issued at system prompt

```bash
history
```
---
### `jobs`, `fg`, `bg`
### `kill`
### `last`
### `less`
### `ln`
### `locate`/`updatedb`
### `ls`
List the files and subdirectories in a directory

```bash
ls
```

Options
* `-F` List the difference between files and directories - directories have a slash `/`
* `-l` List files with status/detail information
* `-lt` List file information in long format, sorted by time with newest files or newly changed files appearing first
* `-a` List all the files in a directory including dot files
---
### `man`
### `mkdir`
Make a directory

```bash
mkdir <directory>
```
---
### `more`
### `mv`
Move `file` to `file2`

```bash
mv <file> <file2>
```
---
### `printenv`
### `ps`
### `ps aux`
### `ps elf`
### `pwd`
Print the pathname of the current directory (present working directory)

```bash
pwd
```
---
### `rm`
Remove or delete files

```bash
rm
```
Options
* `-f` Remove the file forcefully.
* `-r <dirname>` Removes all contents of a non-empty directory and the directory itself
---
### `rmdir`
Remove directory

```bash
rmdir <directory>
```
---
### `set`
### `sh`
### `sort`
### `strings`
### `su`
Switch user
```bash
su <user>
```
### `sudo`
Commands that the only root is authorized to execute
```bash
sudo <command>
```
### `touch`
`touch` is used to update the access date and/or modification date of a file or directory. If the file does not exist then it creates a zero byte file.
```bash
touch <filename>
```
### `uniq`
### `wc`
`wc` (**w**ord **c**ount) simply counts the number of words, lines, and characters in the file(s).

`wc [-option] filename`

`wc -l <filename>` This command will display the number of the lines in filename.

### `which`
### `zsh`
