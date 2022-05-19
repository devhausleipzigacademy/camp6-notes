# Command Line Exercises

[Source for Exercises (contains solutions)](https://github.com/scottjoseph/cmd-exercises)

A list of exercises to practice [[Bash]] commands.

## First Command

1.  Write a command that prints out the string “hello, world”. (Extra credit: As in Listing 1, do it two different ways) 
		**- echo hello, world 
1.  Type the command echo ’hello (with a mismatched single quote), and then get out of trouble
		**- just close the shell?**
		**- repeat mismatched single quote
		- /^C does not work for me**

## Directories

1.  Write in words how you might speak the directory ~/foo/bar.
	**- bar is a subfolder of foo which is a subfolder of the home directory** 
2.  In /Users/dnmct/dev, what is the home directory? What is the username? Which directory is deepest in the hierarchy?
	**- the home folder is  /User/dnmct**
	**- username is dnmct**
	**- the deepest directory is dev but do we know if dev is a file or a directory?** 
1.  How do the effects of cd and cd ~ differ (or do they)?
	**- I moved to a subfolder 2 levels away from root and both commands brought me back there so no there is no difference**
2.  Make a directory foo with a subdirectory bar, then rename the subdirectory to baz.
	**- mkdir foo**
	**- mkdir foo/bar**
	**- mv foo/bar/ foo/baz**
3.  Remove foo and everything in it using a single command.
	**- rm -rf foo**

## Renaming, copying, deleting

1.  Use the echo command and the redirect operator > to make a file called foo.txt containing the text “hello, world”. Then, using the cp command, make a copy of foo.txt called bar.txt. Using the diff command, confirm that the contents of both files are the same.
	 **- echo hello, world > foo.txt**
	 **- cp foo.txt bar.txt**
	 **- diff bar.txt foo.txt -> gives no output which I guess is fine -> -s to report identical files**
1.  By combining the cat command and the redirect operator >, create a copy of foo.txt called baz.txt without using the cp command.
	 **- cat foo.txt > baz.txt**
1.  Create a file called quux.txt containing the contents of foo.txt followed by the contents of bar.txt.
	**- cp foo.txt quux.txt**
	**- cat bar.txt >> quux.txt 
	**- OR: cat foo.txt. bar.txt >> quux.txt
1.  Type the sequence of commands needed to create an empty file called foo, rename it to bar, and copy it to baz.
	**- touch foo**
	**- mv foo bar**
	**- cp bar baz**
1.  Remove both bar and baz using a single call to rm
	**- rm bar baz**

## Redirecting and appending

1.  Using echo and >, make files called line_1.txt and line_2.txt containing two different sentences.
	**- echo This is file 1 > line_1.txt**
	**- echo This is file 2 > line_2.txt**
1.  Use cat to combine the contents of line_1.txt and line_2.txt in reverse order using a single command, yielding the file combined_reversed.txt.
	**- cat line_2.txt line_1.txt > combined_reversed.txt**

## Man pages

1.  According to the man page, what is the official description of echo on your system?
	**- The echo utility writes any specified operands, separated by single blank characters and followed by a newline character, to the standard output.**

## Editing the line

1.  Using the up arrow, print to the screen the strings “fee”, “fie”, “foe”, and “fum” without retyping echo each time.

## Cleaning up

1.  Clear the contents of the current tab.
2.  Exit your shell and reopen the terminal.
			**- type exit which closes session but it does not close the window

## Misc

1.  Write a command to print the string Use "man echo", including the quotes; i.e., take care not to print out Use man echo instead.
	**- echo  "Use \"man echo\""**
1.  By running man sleep, figure out how to make the terminal “sleep” for 5 seconds, and execute the command to do so. After waiting the requisite 5 seconds, execute the command to sleep for 5000 seconds, realize that’s well over an hour, and then get out of trouble.
	**- sleep 5**
	**- close terminal or press ctrl + c

## Listing

1.  What’s the command to list all the files (and directories) that start with the letter “s”
	**- ls s*/**
	**- called globbing and is useful for pattern searching**
	
	