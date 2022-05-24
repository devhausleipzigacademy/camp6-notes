List of Commands:

echo -- repeats back the commands
echo "add to file" >new name overrides anything thats there 

which -- searches for a path

man -- manual; accepts the name of other command line tools

man echo -- gives a list of common user commands 

man ls -- gives a list of directory contents 

ls -- list; list files and directories ls. type -a to show hidden files (usually system files with the .prefix)

cd -- change directory; make any changes 

cp -- copy; used to copy files or group of files or directory. It creates an exact image of a file on a disk with different file name.

touch -- create a file and display timestamp of last update (used to create files easily when there isn't already a folder there)

rm--  remove; to delete files. -r lets you delete nested folders

rmdir -- remove; to delete directories

mv -- move; moves a file/folder, can be used to rename a file by just moving it to the same folder

cat -- concatenate; used to view the contents of files

mkdir -- make directory, folders

diff -- difference; shows the diff. between two text files -s flag to check if they're identical 

f-- force;
">" redirecting inputs and outputs

">>" appends specific files, is much more direct and specific 

cd ..  --- .. is an alias for the parent folder

flags are intended to modify behavior 
ls shows the content of a folder -- is an argument and is code![[Screenshot 2022-05-06 at 15.37.27 1.png]]

General Usage Notes:

*  up and down arrows lets you navigate through history of executed commands
* the 'clear' command clears your screen of contents
* q to quit 



Shorthands for Relative Path

cd . takes you back to the same folder you're in
cd .. this takes you back to the parent folder
cat vs cd ?????? 


understanding a different in files using diff:
a c d 
addition, change, deletion

\\\ use backslashes to escape the next character from being interpreted by the shell

![[Screenshot 2022-05-09 at 12.02.49.png]]

how to search for files placeholder* for example f* will show anything that starts with f