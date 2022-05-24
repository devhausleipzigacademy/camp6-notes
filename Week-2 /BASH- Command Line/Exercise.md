# Command Line Exercises

## First Command

1.  Write a command that prints out the string “hello, world”. 

`echo "hello, world"`

2.  Type the command echo ’hello (with a mismatched single quote), and then get out of trouble

control +c 

## Directories

1.  Write in words how you might speak the directory ~/foo/bar.
home, foo, bar 

2.  In /Users/dnmct/dev, what is the home directory? What is the username? Which directory is deepest in the hierarchy?

home is users, username is dnmct, deepest is dev

4.  How do the effects of cd and cd ~ differ (or do they)?
   
They don't?

6.  Make a directory foo with a subdirectory bar, then rename the subdirectory to baz.

`mkdir foo`     `mkdir foo/bar`   `mv foo/bar foo/baz`

7.  Remove foo and everything in it using a single command.

`rm -rf foo`


## Renaming, copying, deleting

1.  Use the echo command and the redirect operator > to make a file called foo.txt containing the text “hello, world”. Then, using the cp command, make a copy of foo.txt called bar.txt. Using the diff command, confirm that the contents of both files are the same.

`echo "hello, world" > foo.txt`      `cp foo.txt bar.txt`      `diff foo.txt foo.bar`

2.  By combining the cat command and the redirect operator >, create a copy of foo.txt called baz.txt without using the cp command.

`cat foo.txt > baz.txt`
  
3.  Create a file called quux.txt containing the contents of foo.txt followed by the contents of bar.txt.
   
`cat foo.txt bar.txt > quux.txt`

4.  Type the sequence of commands needed to create an empty file called foo, rename it to bar, and copy it to baz.

`touch foo`, `mv foo bar`, `cp bar baz`   
   
5.  Remove both bar and baz using a single call to rm
   
`rm ba*` 

## Redirecting and appending

1.  Using echo and >, make files called line_1.txt and line_2.txt containing two different sentences.

`echo "Hello my name is Suzy" > line_1.txt` , `echo "I do not really know what I am doing" > line_2.txt`   
   
2.  Use cat to combine the contents of line_1.txt and line_2.txt in reverse order using a single command, yielding the file combined_reversed.txt.

## Man pages

1.  According to the man page, what is the official description of echo on your system?



## Editiing the line

1.  Using the up arrow, print to the screen the strings “fee”, “fie”, “foe”, and “fum” without retyping echo each time.

## Cleaning up

1.  Clear the contents of the current tab.
2.  Exit your shell and reopen the terminal.

## Misc

1.  Write a command to print the string Use "man echo", including the quotes; i.e., take care not to print out Use man echo instead.
2.  By running man sleep, figure out how to make the terminal “sleep” for 5 seconds, and execute the command to do so. After waiting the requisite 5 seconds, execute the command to sleep for 5000 seconds, realize that’s well over an hour, and then get out of trouble.

## Listing

1.  What’s the command to list all the files (and directories) that start with the letter “s”