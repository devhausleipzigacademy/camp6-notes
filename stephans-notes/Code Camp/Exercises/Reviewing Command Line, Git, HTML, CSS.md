# Review Questions

## Command Line

1. What command clears the contents of your terminal display?
	- clear

2. What is the command to delete a file?
	- rm

3. What command is used to change directories?
	- cd

4. What do you type in to move to the parent directory?
	- ..

5. What command is used to copy a file?
	- cp

6. What command shows you what directory you are in?
	- ls

7. What command creates an empty directory?
	- mkdir

8. What command displays your current username?
	- whoami

9. What command is used to change a file name?
	- mv

10. What is the command to run a program with elevated permissions?
	- sudo (superuser do)

11. What is the command to print out the contents of a file to the terminal?
	- cat

12. Which option with the command "rm" is required to remove a directory?
	- d or r or simply use "rmdir"

13. The command used to display the manual pages for any command is?
	- man

14. Which option of "ls" will show the hidden files?
	- a

15. How do you quit VIM?
	- enter command mode (press esc) and type ":q"

16. How do you save before quitting VIM?
	- enter command mode (press esc) and type ":wq"

  

## Git

1. What's the git command that downloads your repository from GitHub to your computer?
	- git pull or git clone

2. What's the opposite of git clone, instead of downloading your code from GitHub, uploads your changes and code back to GitHub?
	- git push after creating repository on github and connecting it

3. What command displays the difference between the working tree and the stage/index area, as well as files not tracked by Git?
	- git status

4. How do you stage files for a commit?
	- git add NameOfFile

5. How do you save the current state of your code into the git version control?
	- git commit

6. What's a shortcut to staging all the changes you have?
	- git add .

7. How do you supply a commit message to a commit?
	- git commit -m

8. What comes first, staging with git add . or committing with git commit?
	- staging comes first

9. Which of the following is the correct way to initialize a new Git repository?
	- git init

10. We've just created a new file called index.html. What command will stage this one file so we can commit it?
	- git add index.html

11. To stage only files with a .txt extention, the command is?
	- git add *.txt

12. Assuming a remote reposistory exists at https://github.com/myawesomegitname/my_repo.git, how would you add the repository as a remote to your local repository?
	- git remote add origin url

13. To get the lastest changes from your remote repository, the git command is?
	- git pull

14. To make a new git branch, the git command is?
	- git branch

15. To make a new git branch and switch to it at the same time, the git command is?
	- git checkout -b NameOfNewBranch

16. To set a local branch to track a remote branch, the command is?
	- git branch -u nameofremotebranch (i guess)
	- alternatively, git push -u remotename branchname

17. Where are files stored before they are committed to the local repository?
	- in the working directory (staging area is only pointer of what to include in commit)

18. Which command is used to integrate changes from one branch into another?
	- git merge

19. How many individual commits can a single repository have?
	- endless

## HTML

1. What is the correct HTML element for the largest heading?
	- h1

2. What is the correct HTML element for inserting a line break?
	- hr

3. What is the correct HTML element to define important text?
	- strong or em

4. What is the correct HTML element to define emphasized text?
	- em

5. What is the correct HTML for creating a hyperlink?
	-  <a href="url">name of web address</a>

6. Which character is used to indicate an end tag?
	- backslash

7. Inline elements are normally displayed without starting a new line?
	- yes?

8. How can you make a numbered list?
	- li elements nested inside ol tags

9. How can you make a bulleted list?
	- li elements nested inside ul tags

10. What is the correct HTML for inserting an image?
	- <img src="url" alt="text if image cannot load" >

11. HTML comments start with <!-- and end with -->?
	- yes

12. Block elements are normally displayed without starting a new line?
	- no

13. Which HTML element defines the title of a document?
	- title nested inside head

14. Which HTML attribute specifies an alternate text for an image, if the image cannot be displayed?
	- alt

15. Which part of an HTML element allows you to define navigation links within a document?
	- a hyperlinks linking to id 

16. Which HTML element is used to specify a header for a document or section?
	- h1 to h6
  

## CSS

1. What CSS property is used to make the text in an element bold?
	- font-weight

2. How do you add a comment in a CSS file?
	- /* this is a comment */ (i.e. backslash asterisk comment asterisk backslash)

3. What property is used to change the text color of an element?
	- color

6. How do you make a list not display bullet points?
- list-style:none

7. What CSS property is used to change the font of text in an element?
	- font-family

8. Which HTML attribute is used to define inline CSS styles?
	- style

11. Which CSS property controls the text size?
	- font-size

12. Which property is used to change the background color?
	- background-color

13. How do you display hyperlinks without an underline?
	- text-decoration: none

14. How can you created rounded corners using CSS?
	- border-radius

15. What property do you use to create spacing between HTML elements?
	- margin

16. What property would you use to create space between the element’s border and inner content?
	- padding

17. How would you style an element so that the next element would appear right next to it, not underneath it, if both elements widths were collectively smaller than the container element?
	- display: inline

19. How would you create a border only below an HTML element?
	- border-bottom

20. If you wanted to put an HTML element at a certain position on the page regardless of the other elements, what value would you give the position property?
	- absolute
