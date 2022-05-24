# Globbing-syntax-exercises
Globbing syntax exercises in the context of .gitignore and Git repos

## Outline

See the GNU globbing reference below for the more general BASH globbing syntax.

### Focusing on the variant of globbing used in .gitignore files

- Comment line: #
	- text preceded by hashtag will be ignored 
- Path section separator: /
- Single character wildcard: ?
	- only stands for a single slot
- Character set and ranges: \[ ][ - ]
	- only stands in for a single slot
	- square brackets can be used to list letters to be ignored, e.g "my-little-project/1/m[aeiou]m" ignores all files in that folder starting and end with m and having a vowel as second letter
	- dash can be used only in square brackets to indicate range, either letters (e.g. a -g) or numbers (e.g. 1-5)
- Wildcard: \*
	- can take on any value 
- Globstar: \*\*
	- can stand in for any path section
- Negative glob: !
	- exclude specified file from being included in gitignore

### General Rule
**It is not possible to re-include a file if a parent directory of that file is excluded**

## Double Checking Gitignore rules working properly

- use command git add ProjectFolder
- git status and check that the right files or in- or excluded
- git reset to undo add

## Resources

- [gitignore - Git Documentation](https://git-scm.com/docs/gitignore)
- [GNU Globbing Reference](http://tldp.org/LDP/GNU-Linux-Tools-Summary/html/x11655.htm)

## Getting the .gitignore highlighting to work on VSCode for these exercises
- `git reset`
- `git rm -rf my-little-project`
- `git commit -m "Remove my-little-project folder"`
- `git checkout HEAD~1 my-little-project`
- `git reset`
