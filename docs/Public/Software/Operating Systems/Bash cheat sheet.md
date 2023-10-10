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