https://devhints.io/bash

```bash
pwd
``` 
- Print working directory, outputs the path to the current directory
```bash
tree <path>
```
- See how the child files are organized from the current directory
```bash
cd <path>
```
- Change directory, changes current directory to the file path given
```bash
ls <path>
ls -a <path>
```
- Lists the files contained in current directory
	- Use `-a` to show hidden files
```bash
mkdir <flags> <path(s)>
```
- Makes directory, a new directory at the file path given
```bash
mv <flags> <sourcePath(s)> <destinationPath>
```
- Moves files from source to destination
	- Can rename / overwrite files
```bash
cp <flags> <sourcePath(s)> <destinationPath>
```
- Copy files / directories
	- Can overwrite existing files
```bash
rm <flags> <filePath(s)>
```
- Remove each specified file permanently
		- Does not remove directories by default
```bash
alias <aliasName>='<commandToRun>'
```
- Substitutes the alias name with the command to be run
	- Create shortcuts for tedious commands
	- Extend the default behavior of commands
```bash
alias rm='rm -i'          # confirm to delete file
alias rm='mv -t -/.tash'  # move file to a trash directory
alias cp='cp -b'          # make backup of destinationFile
alias mv='mv -u'          # move only if sourceFile is newer
alias hello="echo 'cow power'"
```

```bash
cat <flags> <file>
less <flags> <file>
```
- Print contents of file to screen; concatenate
	- `less` outputs a page at a time, to scroll through
	- Can search through file using the `/<word>` 
```bash
head <flags> <file>
```
- Shows the first 10 lines of a file
	- Use `-n <number of lines>` to print certain number of lines from file
```bash
tail <flags> <file>
```
- Shows the last 10 lines of a file
```bash
nano <flags> <file>
```
- Opens simple [[CLI]] text editor
```bash
vim <flags> <file>
```
- Another text editor
```bash
man <command>
man mkdir
man stdio
```
- System reference manuals
- Contains details of all command behavior and flags
- Documentation of c libraries
```bash
tldr <flags> <command>
```
- Lists the typical uses of a command

```bash
grep 'word-to-search' <file_name>
grep 'word-to-search' <file_name1> <file_name2> <file_name3> ...
grep 'pattern' <file_name>      # searches by regex pattern
```
- Searches the given files for lines containing a match to a given pattern list [^1]

```bash
grep 'Gandalf' list_of_dwarves.txt 

if [[ $? != 0 ]] 
then 
	echo "Gandalf is not a dwarf" 
	exit 1 
else 
	echo "Gandalf is a dwarf" 
	exit 0 
fi
```
- `$?` stores the exit code for the last command

[^1]: https://www.cyberciti.biz/faq/grep-in-bash/

```shell
p10k configure
```
- Configure `powerlevel10k` looks