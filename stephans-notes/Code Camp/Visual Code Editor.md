# Visual Code Editor
Visual Studio Code, also commonly referred to as VS Code, is a source-code editor made by Microsoft for Windows, Linux and macOS. Features include support for debugging, syntax highlighting, intelligent code completion, snippets, code refactoring, and embedded [[Git & Github]]. Users can change the theme, keyboard shortcuts, preferences, and install extensions that add additional functionality.

## Commands
cmd or ctrl + shift + p -> Open the Command Palette  (e.g. open terminal or open settings)
cmd or ctrl + s -> Save File 
Save All Files -> no keybindings (default on Mac)
cmd or ctrl + shift + e -> Show Explorer 
cmd or ctrl + 1 -> Focus First Editor Group 
cmd or ctrl + w -> Close Editor 
cmd or ctrl + K cmd or ctrl + W -> Close All Editors
^C -> Create New integrated Terminal -> no keybindings (default on Mac DE)
cmd or ctrl + 0 -> Focus Into Sidebar 
cmd or ctrl + f -> Find  
alt + arrow key (up or down) -> Move Line Up & Move Line Down 
^ + R -> Open Recent...
cmd + N -> open new window
cmd + shift + N -> open new tab
cmd + W -> close tab
cmd + shift + W -> close window
cmd + shift + T -> reopen closed editor
cmd + K P -> copy path of active file
^ cmd + F -> toggle full screen 
cmd + K O -> Zen mode (Esc to exit)

[Full List of Commands](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf) -> Warning: the list is for Mac OS specifically; type help keyboard into Command Palette to find a list for your device

# VS Code Shortcuts
- command shift + e -> show explorer
- command 0 -> focus sidebar
- command + numbers -> switch editor groups 
- control + numbers -> switch tabs
- command + arrow key -> move line up or down

## Text editing shortcuts
- command arrow key ->
- option arrow key ->
- command or control shift arrow key ->

⌘X Cut line (empty selection)  
⌘C Copy line (empty selection)  
⌥↓ / ⌥↑ Move line down/up  
⇧⌥↓ / ⇧⌥↑ Copy line down/up  
⇧⌘K Delete line  
⌘Enter / ⇧⌘Enter Insert line below/above  
⇧⌘\ Jump to matching bracket  
⌘] / ⌘[ Indent/outdent line  
Home / End Go to beginning/end of line  
⌘↑ / ⌘↓ Go to beginning/end of file  
⌃PgUp / ⌃PgDn Scroll line up/down  
⌘PgUp /⌘PgDn Scroll page up/down  
⌥⌘[ / ⌥⌘] Fold/unfold region  
⌘K ⌘[ / ⌘K ⌘] Fold/unfold all subregions  
⌘K ⌘0 / ⌘K ⌘J Fold/unfold all regions  
⌘K ⌘C Add line comment  
⌘K ⌘U Remove line comment  
⌘/ Toggle line comment  
⇧⌥A Toggle block comment  
⌥Z Toggle word wrap

## Documentation

[VS Code Documentation](https://code.visualstudio.com/Docs)

## Tips & Setup

- useful additions to setup JSON
	>"prettier.useTabs": true, "terminal.integrated.fontFamily": "FiraCode NF", "editor.fontLigatures": true, "editor.fontSize": 16, "editor.wordWrap": "on", "debug.console.fontSize": 16, "workbench.settings.editor": "json", "git.autofetch": true, "editor.formatOnSave": true, "editor.defaultFormatter": "esbenp.prettier-vscode"

### Set up Format on Save 
One of the most helpful features of Visual Studio Code is the ability to have code be automatically formatted on every change. Here are the steps to configure this 
1. Go to the extensions and install an extension called **Prettier - Code formatter** 
2. 2. Open the user settings and set the setting `editor.formatOnSave` to true. 
3. Also set the `editor.defaultFormatter` to be prettier. 
4. Try it out by opening up an markdown document, messing with the indentation and hitting the keyboard shortcut to save. You should see your code automatically jump back into place 

### Other Extensions 
- indent-rainbow (you should also change your prettier settings 'Use Tabs') 
- quokka
- live preview (to preview html inside VS Code)