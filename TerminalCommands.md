---
Title: Command Line
Author: Ling
---



# Sources & References
- [Official Ububtu Tutorials](https://ubuntu.com/tutorials/command-line-for-beginners)
- [Linux Shell Commands](https://docs.cs.cf.ac.uk/notes/linux-shell-commands/)
- [Cheat Sheet by Tahul Saigal](https://www.makeuseof.com/tag/mac-terminal-commands-cheat-sheet/)
- [Mac Homebrew](https://pastebin.com/jV9XzPrs)

# Useful Tools


## Remote Connection Environment

|Commands| Results|
| --- | --------- |
| `ssh username@server.address`|Connect to remote server
| `export LC_ALL="en_US.UTF-8" `|Set language
| `module load r/3.5.0-py2-x335hrh`| Load a specific environment
| `qstat -a`| All jobs
| `qstat -u username`| Jobs submitted by user
|  `qsub` | Execute the jobfile
|   `qdel` | Terminate one job

## Editing using terminal editor
|Commands| Results|
| --- | --------- |
|   `nano <file>` | Open the terminal editor to write file
|  control + x | Exit the terminal editor 

## Testing using terminal R environment

1. Load R module: `$ module load r`
2. Enter R environment:  `$ R`
3. Exit: `q()`

## Homebrew & Cask
Useful to install and version control softwares.
|Commands| Results|
| --- | --------- |
|` xcode-select —install`|Install Xcode Tools
|`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`|  Install Homebrew

|Commands| Results|
| --- | --------- |
|`brew install cask`| Install Cask
| `brew search --casks`| List apps
|  `brew search (discord)  `|  Search apps
| `brew cask install (discord)`|Install
|` brew cask upgrade`|Update all softwares downloaed through cask
|` brew cask help`|Help

## Short Cuts
|Commands| Results|
| --- | --------- |
|    Ctrl + A	| Go to the beginning of the line you're currently typing on
|    Ctrl + E	| Go to the end of the line you're currently typing on
|    Ctrl + U	| Clear the line before the cursor
|    Ctrl + K	| Clear the line after the cursor
|    Ctrl + C	| Kill whatever you're running
|    Ctrl + D	| Exit the current shell
## Basic Commands
|Commands| Results|
| --- | --------- |
|   ` / (Forward Slash)`|	Top level directory
|    `. (Single Period)`|	Current directory
|   `.. (Double Period)`|	Parent directory
|   `~ (Tilde)`	|Home directory
|  `sudo [command]`	|Run command with the security privileges of the super user
|   `nano [file]`	|Opens the Terminal editor
|   `open [file]`	|Opens a file
|   `[command] -h`	|Get help about a command

## Change Directory (cd)
|Commands| Results|
| --- | --------- |
| `cd` |	Home directory|
| `cd [folder]`|	Change directory, e.g. cd Documents|
| `cd ~	` | Home directory|
|`cd/`|	Root of the drive|
| `cd -`|	Previous directory or folder you last browsed|
| `pwd` |Show your working directory|
|`cd..` |Move up to the parent directory|
|`cd../..`|	Move up two levels|

## List (ls)
|Commands| Results|
| --- | --------- |
|   `ls`|	Display the name of files and subdirectories in the directory
|  `ls -C`	|Force multi-column output of the listing
|   `ls -a`	|List all entries including those with .(period) and ..(double period)
|   `ls -l <dir/file>`	|List the sizes of the files in the dir / files, use * to list all the file sizes in the current dir
|   `du -sh .`	|Calculate the whole size of the current dir


## File and Directory Management
|Commands| Results|
| --- | --------- |
| `mkdir <dir>`	| Create new folder named <dir>
| `mkdir -p <dir>/<dir>`	| Create nested folders
| `mkdir <dir1> <dir2> <dir3>`| 	Create several folders at once
| `mkdir "<dir>"`| Create a folder with a space in the filename
| `rmdir <dir>`	| Delete a folder (only works on empty folders)
| `rm -R <dir>`	| Delete a folder and its contents, equivalent to `rm -r`
| `rm <file>`	| Delete a file (This deletes the file permanently; use with caution.)
| `rm -i <file>`	| Delete a file only when you give confirmation
| `rm -f <file>`	| Force removal without confirmation
| `rm <file1> <file2> <file3>`	| Delete multiple files without any confirmation
| `mv <file> <newfilename>`	| Move/rename
| `mv <file> <dir>`	| Move a file to the folder, possibly by overwriting an existing file
| `mv -i <file> <dir>`	| Optional -i flag to warn you before overwriting the file
| `mv *.png ~/<dir>`	| Move all PNG files from current folder to a different folder
| `touch <file>`	| Create a new file without any extension
| `cp <file> <dir>`	| Copy a file to the folder
| `cp <file> <newfile>`	| Copy a file to the current folder
| `cp <file>~/<dir>/<newfile>`	| Copy a file to the folder and rename the copied file
| `cp -R <dir> <"new dir">`	| Copy a folder to a new folder with spaces in the filename
| `cp -i <file><dir>`	| Prompts you before copying a file with a warning overwrite message
| `cp <file1> <file2> <file3>/Users/<dir>`	| Copy multiple files to a folder

