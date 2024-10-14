# Making VS Code Awesome

Ctrl + ~ to open Terminal

# UI

Activity Bar - on the side
Status Bar - at the bottom
Panels - where the files show up
Minimap - file overview on right side of pane
Side by Side Editing - Have two panes of same file |---| symbol at top right of file. Command pallete split editor.
                                                   | | |
                                                   |---|

# Minimalism

 Cmd/Ctrl + Shift + P: Toggle Zen Mode
 Cmd/Ctrl + Shift + P: Toggle Centered Layout
 Cmd/Ctrl + Shift + P: go to ... symbol, file, etc.

## Main UI Minimalism
Render Indent Guides - off
  "editor.RenderIndentGuides": false
Workbench Activity Bar Visible - off
  "workbench.activityBar.visible": false
Workbench Status Bar Visible - off
  "workbench.statusBar.visible": false
Editor Minimap Enabled - off
  "editor.minimap.enabled": false
Explorer Open Editors Visible - off
  "explorer.openEditors.visible": false

!!!!! You can move the Activity Panel to the right side !!!!!

## Tabs UI Minimalism
  "workbench.editor.showIcons": false,
  "workbench.editor.tabCloseButton": false,
  "workbench.editor.showTabs": false,

## Gutter UI Minimalism (gutter is to the left of the file, line number, debug poins, etc.)
  "editor.lineNumbers": false,
  "editor.glyphMargin": false,
  "editor.folding": false,

# Productivity
Settings: Files: autosave - afterDelay
Settings: Files: autosave delay - 1500 milliseconds
Extensions: Prettier
  - settings: default formatter: prettier
  - settings: format on save - WARNING: Autosave doesn't format, you have to do Cmd/Ctrl + S to autoformat.

# Extensions
NOTE: You can disable extensions per workspace. vs code can get slow with too many extensions
NOTE: .vscode/ for workspace can hold recommended extensions for the project. open command pallete and type recommended extensions to modify

Browser - !!! Browser Preview !!!
  - Settings: Browser preview: Start URL

Theme - Winter is Coming
Theme - !!!! Ocean Green Dark !!!!
Theme - minimalGreen
Theme - Monokai Pro
Theme - Moonlight and Moonlight II
Theme - Material
Theme - Panda
Icon Theme - Material Icon Theme
Intellisence - for python. Alt + Space to get intellisense. Needs Python extension
Python
Prettier - code formatting
Vim and amvim - amvim is more minimal. Vim extension throws you into the world of vim in vs code; not great.
  - Vim has movement mode and edit mode which is why it's powerful. Helpful for moving around files efficiently
Don't forget emacs extension

# Terminal
Try using GitBash in Windows - will need to redo python anaconda environments

settings: terminal font size
settings: terminal line height spacing
settings: terminal external - to change the shell

# Git

settings: Default clone directory
Extension: Git History
Extension: Git Indicators - shows number of files changed in botton status bar
Extension: GitLens - the big one
Extension: Git Blame
Extensions: gitlink

# Fonts - NOTE: you have to install fonts, look up how to do that.

coding-fonts.css-tricks.com

* Dank Mono
* [Monokai Pro](https://monokai.pro/vscode)
* Fira Code
* Fira Flont
* Cascadia Code by Microsoft
* Operator Mono - Great, expensive
* Lotion

# Working with multiple projects

Extension: Project Manager

# Settings
NOTE: Settings sync: You can sign in to microsoft or github to sync settings across computers

Line Height
Font size
Ligatures
Mouse wheel zoom - Ctrl + scroll wheel to zoom. False by default
tab size
rulers - set to 120 line length
render indent guides - off better
word wrap - off by default
word wrap column - set to 120 or 80
editor: cursor blinking
Editing Preview: True by default. set to false !!!
Workbench Startup Editor: Open untitled file is best
Default Language: Markdown so you can take notes
search exclude

# Editing

settings: Editor: Cursor Smooth Caret Animation - ON  !!!! 
Explorer - Outline - shows an outline of the file you have open
Extension - advanced-new-file - create new file through command pallete
Multi-Cursor Editing - Cmd/Ctrl + F, then Option/Alt + Enter once you've searched for something

# Keyboard Shortcuts

Help: Cmd/Ctrl + K then Cmd/Ctrl + R - For a Keyboard (K) Reference (R)
Help: Keyboard Shorcuts: Cmd/Ctrl + K then Cmd/Ctrl + S


Cmd/Ctrl + N - New file
Cmd/Ctrl + W - Closes File
Cmd/Ctrl + \ - split editor for same file - Cmd + 1 for first file and Cmd + 2 for second file
Cmd/Ctrl + Shift + T - open a closed tab (say a file)
Cmd/Ctrl + X - cut line
Option + down arrow - move line down
Option + up arrow - move line up
Shift + Option + down arrow - copy lines down
Cmd/Ctrl + / - hightlight lines, will comment out all lines.
Cmd/Ctrl + Enter - new line below
Cmd/Ctrl + Shift + Enter - new line above

## Navigation

Cmd/Ctrl + G: Type line 50, hit enter, jumps there
Cmd/Ctrl + O: type symbol name, jump there
F12 - go to definition

## Command Pallete

">" - means show command VS code has
":" - means go to line number
"@" - will find symbols 

## Multi-cursor
Shift + Option and use mouse to multiselect across lines
Option + Click down to select multiple lines
Cmd/Ctrl + D - select next instance of same text that's already hightlighted.

## Misc
Command or Ctrl B - close left side bar
F12 - go to definiteion of function
Cmd/Ctrl + Shift + F - find and replace in files
F2 - Rename symbol - rename across entire file system.
Cmd/Ctrl + W - close a file
Control^/Alt + ~  - open terminal
Cmd/Ctrl + P - open a file
Cmd/Ctrl + O - find a symbol in a file

# Click Shortcuts

Right-Click - find all references
Right-Click - rename symbol - works across multiple files
Right-Click - Peek to bring up snippet of function. You can even edit it.

# Searching

Get a rich files search by clicking the +new seach window icon in the Cmd/Ctrl + Shift + F pane.

# Snippets

Open extensions and search @category:"snippets" python

fo + TAB should give you options to fill in for loop
docstrings would be nice, look that up

Extension: autoDocString

Code/User/Snippets/ - put your own snippets here

# Code command line interface (CLI)

command pallete - install 'code'

# Markdown

Preview markdown with button in top right of .md file |---|
                                                      | | |
                                                      |---P

Extension: Markdown all in one
 - Just paste on highlighted test and a link is inserted
 - Cmd/Ctrl + Shift + P: "Markdown Create Table of Contents" - automatically inserts table of contents
Extension: Markdownlint
Extension: Markdown Preview Github Styling - just changes markdown preview to look like github

# API Calls - Make a REST call and get the response in VS Code
Extension: Thunder Client
