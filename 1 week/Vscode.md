Create a note called `VSCode` in which you list handy commands and their corresponding keyboard shortcuts. Use the command palette to find out to which keys these commands are mapped. You are free to include as many keyboard shortcuts as you like, but make sure to at least include these: 
- Open the Command Palette 
- - Save File
- Save All Files
- Show Explorer
- Focus First Editor Group
- Close Editor
- Close All Editors
- Create New integrated Terminal
- Focus Into Sidebar
- Find
- Move Line Up & Move Line Down
- Open Recent... If you have included those, open the command palette and look for Help: Keyboard Shortcut Reference to open the printable keyboard cheatsheet. Test the different commands and pick the ones you find most useful to your list. 
  
## Set up Format 
on Save One of the most helpful features of Visual Studio Code is the ability to have code be automatically formatted on every change. 

Here are the steps to configure this 

1. Go to the extensions and install an extension called  **Prettier - Code formatter** 
2. Open the user settings and set the setting `editor.formatOnSave` to true. 
3. Also set the `editor.defaultFormatter` to be prettier. 
4. Try it out by opening up an markdown document, messing with the indentation and hitting the keyboard shortcut to save. You should see your code automatically jump back into place ## Other Extensions - indent-rainbow (you should also change your prettier settings) - quokka





"prettier.useTabs": true, "terminal.integrated.fontFamily": "FiraCode NF", "editor.fontLigatures": true, "editor.fontSize": 16, "editor.wordWrap": "on", "debug.console.fontSize": 16, "workbench.settings.editor": "json", "git.autofetch": true, "editor.formatOnSave": true, "editor.defaultFormatter": "esbenp.prettier-vscode"
