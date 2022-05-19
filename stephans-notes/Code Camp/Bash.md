# Bash
Bash is a shell program for the Command Line

every command in bash is basically a separate program that is executed on command

### To do 
- add a definition for command line#
- create a table for commands
- check if there is a difference between command modifier, option, and flag

## Commands
| Input | Output | Modifier | Example

echo -> repeats input e.g. echo "hello world" = hello world; also writes text into a file, e.g. echo "hello world" > exampleFile1
ls -> lists content of folder that I am in
ls -a -> lists content including hidden files
which -> gives location of succeding command e.g. which echo
man echo -> lists modifier and explains function of succeding command
clear -> clears screen of content
mkdir -> creates folder with name of succeding argument e.g. mkdir exampleFolder
cd -> changes directory, e.g. cd exampleFolder moves user into folder exampleFolder
touch -> update or modify file or more often create new file if there is no file with given name already e.g. touch exampleFile1
cat -> prints content of file given as argument e.g. cat exampleFile1 ( can be used to print content to screen or file)
rm -> removes whatever file is listed as argument rm exampleFile1
rmdir -> removes folder listed as argument e.g rmdir exampleFolder
rm rf -> "r" (recursive) allows to delete nested folders, "f" (forced) allows to delete files as well
mv -> moves (or renames which is essentially the same) a file from one place to another
diff -> shows difference between two text files (will provide details of difference e.g. "2a3" says second file has an addition in line 3; "1c1, 3" says first file has change in lines 1 and 3)
nano -> opens text editor
cp -> copy

. represents present folder e.g. cd . will mean you stay in same folder
.. represents parent folder e.g. cd .. will move you to present folder

can add argument to command e.g. echo "hello world" -> hello world is argument
can add modifier/option or flag to command

tab can be used to autocomplete
if multiple options available double tab will list all options

operator > delineates direction, e.g. echo "hello world" > exampleFile1 the operator tells the command where to print the argument (seems to be know as redirect operator)
	- redirect will override previous content
	- use append operator to append data in file >> e.g. echo "this too will fade" >> exampleFile1 -> exampleFile1 reads "Hello world this too will fade"
	- append only works with files, redirect works with directories too

## command line vs operator

- command line is program executed via shell 
- operator is tool used and provided by shell itself
