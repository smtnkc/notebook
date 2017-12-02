# My Favorite VS Code Shortcuts & Extensions

> **Note:** In addition to VS Code specific shortcuts, I am using the scroll keys
**`Home`**, **`End`**, **`Page Up`**, **`Page Down`** quite often. I combine them with additional
**`Delete`** and **`Shift`** keys. That is why I like to use an **enhanced PC keyboard**.

### For clarification:
* **`F1`** display all commands and shortcuts in VS Code.
* **`MC`** Mouse-click (Left)
* **`🠅`** Up arrow key
* **`🠆`** Right arrow key
* **`🠇`** Down arrow key
* **`🠄`** Left arrow key
### File Navigation
* **`Ctrl +`**
  * **`B`** toggle explorer
  * **`J`** toggle panel (terminal)
  * **`W`** close file
  * **`Tab`** navigate between open files
  * **`P`** navigate between project files
    * Use **`Enter`** to directly open file
    * Use **`🠆`** to add file to open files
    * Use **`Ctrl + Enter`** to open file in a splitted tab
    * Append **`:N`** to the search keyword to jump line **N**
* **`Ctrl + Shift +`**
  * **`F`** search a keyword in project
  * **`E`** show project files in explorer
  * **`G`** show Git (source control) in explorer

### Text Selection & Editing
* **`Shift + Delete`** cut line
* **`Alt + 🠅🠇`** move line to up or below
* **`Alt + MC`** put additional cursors to clicked area for editing
* **`Alt + Shift + 🠅🠇`** pug additional cursors to upper/below line for editing
* **`Alt + Shift + 🠆`** select all of the child content
  * Press **`🠆`** multiple times to extend the selection
  * Press **`🠄`** multiple times to shrink the selection
* **`Ctrl +`**
  * **`🠄🠆`** jump word by word
  * **`Shift + 🠄🠆`** select word by word
  * **`Delete`** or **`Backspace`** delete word by word
  * **`Shift + I`** auto format code
### Extensions
Coming soon...

### settings.json
```json
{
    "editor.fontSize": 16,
    "editor.fontWeight": "normal",
    "workbench.panel.location": "bottom",
    "workbench.colorTheme": "One Dark Pro",
    "workbench.startupEditor": "newUntitledFile",
    "editor.fontFamily": "SF Mono",
    "terminal.integrated.fontFamily": "SF Mono",
    "workbench.iconTheme": "material-icon-theme",
    "explorer.confirmDelete": false,
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/CVS": true,
        "**/.DS_Store": true,
        "node_modules": true,
        ".vscode": true,
        "package-lock.json": true
    },
    "editor.renderWhitespace": "boundary",
    "workbench.colorCustomizations": {
        "editorWhitespace.foreground": "#626462"
    }
}
```
