# VS Code intro

For this intro to work, one is expected to have `node` and `python` installed, as well as some specific VS Code extensions.

If one does not wish to install these, one can instead launch a VS Code Dev container from this directory. That container will have dependencies installed.

## Intro

[link](https://code.visualstudio.com/docs/introvideos/basics)

This link goes through basic VS Code features.

- How to use intellisense with `js` files
- How to use intellisense with `python` after adding the Python extension
- How to preview `html` files after adding the Live Preview extension

## Code Editing

[link](https://code.visualstudio.com/docs/introvideos/codeediting)

This video shows examples for `node`

## Productivity Tips

[link](https://code.visualstudio.com/docs/introvideos/productivity)

Covers:

- Command palette
- Quick open file
  - Add colon to open at line number
  - Add at sign to go to the symbol
  - Use question mark to look for command suggestions
  - Use right arrow key to open file but keep the menu open for opening more files
- Multi-cursor
  - with `alt` click
  - `ctrl` + `alt` + up or down arrow
  - `shift` + `ctrl` + `l` to select all instances of word under the cursor
- Formatting and saving automatically
  - on typing, on saving, on pasting, for example
- Intellisense
  - by default for javascript. For example, type an object then a dot to see all methods available.
  - Triggered with `ctrl` + `space` in any window

## Personalize VS Code

[link](https://code.visualstudio.com/docs/introvideos/configure)

- UI theme
- icon theme

## Extensions

[link](https://code.visualstudio.com/docs/introvideos/extend)

- Themes are offered by extensions
- Can use at symbol when searching marketplace for key words
  - For example, using `@installed`
- Language extensions needed for many extensions, for example for `python`
- Can use command palette to search for commands offered by an extension
- VS Code may recommend extensions based on your context, as well. For example, if you create a `.java` file, you may be prompted to install extensions for that programming language.

## Debugging

[link](https://code.visualstudio.com/docs/introvideos/debugging)

- Shows debugging for `node` and `python`
- Using `F5` will try to debug, and you may need to specify debugging parameters if VS Code does not detect them automatically
  - Using `app.js`, you should be able to see your app in localhost:3000
- Can modify the 'launch configurations' by modifying the `.vscode/launch.json` file
  - Can use intellisense to get suggestions for configurations. For example, you may want to pause the debugger as soon as it has launched using the `"stopOnEntry": true`
- Features in debug menu include:
  - Play button to debug in different configurations
  - Gear icon to open the configuration file
  - Variables
  - Watch
  - Call Stack
  - Loaded Scripts
  - Breakpoints
  - ... menu to customize sidebar
  - Debug Console
  - Orange color change indicates you are in debug mode
  - Buttons at top of debug toolbar:
    - Continue/pause
    - step over
    - step into or out of a function call
    - restart
    - stop
- All languages that are transpiled to javascript are supported out-of-the-box in VS Code. Other languages require other installations.
  - Can be done from 'Run -> Install additional debuggers' to search the extensions marketplace using `@category:debuggers`
- Breakpoints allow you to interrupt code execution at a specific place. Use `F9` to set one wherever your cursor is in a given file.
  - Once a program is paused, hovering over items allows you to interrogate their values at the moment the program was paused.
  - Step over allows you to proceed
  - Step into allows you to investigate a function, for example

## Version control

[link](https://code.visualstudio.com/docs/introvideos/versioncontrol)

- Can initialize a repository from the UI (`git init`)
- Can rename the branch from the UI also (`git <branch> -m <new name>`)
- Can commit and add messages from the UI (`git commit -m '<message>'`)
- Can make a new branch from the UI (`git checkout -b <new-branch>`)
- The UI indicates with gray, blue, or red colors in the 'gutter' to indicate the kinds of changes that have not yet been staged.
- VS Code UI allows you to compare files side-by-side, or using 'in-line' view
- Can merge branches in the UI also
- Can publish branches from the UI (if first time, will give you option to do public or private repository)
  - To do this from the command line would require installation of the GitHub command line tool, in addition to `git`, since you cannot create a GH repository with `git` alone
- Can use the UI to clone a repository as well (`git clone <URL>`)

## Customize

[link](https://code.visualstudio.com/docs/introvideos/customize)

- Keyboard shortcuts
  - Can see keyboard shortcuts listed when searching items in the command palette
  - Can use gear icon next to items in the command palette to configure the keyboard shortcut
  - Can view keyboard shortcuts as a JSON as well, which is easiest found from the command palette
  - There are extensions to try to match keyboard shortcuts from other editors (e.g., Vim)
- VS Code settings
  - Two levels: User level, Workspace level
  - Can be viewed via a UI or a JSON
  - Can configure language-specific settings as well
- Can configure settings sync and modify what is synced
  - I have not played enough with this to know if it's easier/more-difficult than simply importing/updating profiles
