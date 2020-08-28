# Improved (IMHO) Key Bindings for the Windows Terminal in Windows 10

## Bindings

### Duplicate pane
#### Auto Horizontal (-) or Vertical (|)
`ALT + SHIFT + D` or `CTRL + D`

#### Horizontal (-)
`CTRL + SHIFT + Down Arrow` or `CTRL + SHIFT + Up Arrow`

#### Vertical (|)
`CTRL + SHIFT + Left Arrow` or `CTRL + SHIFT + Right Arrow`

### Move Focus
`CTRL + Arrow` 

### Close Pane
`CTRL + F4`


## Installation

A little awkward as we have to install into an existing folder.

Find the folder of your existing Windows Terminal settings.json file by copying its path. You can do this by clicking Settings in the Windows Terminal menu which will open the file in a text editor, e.g. VS Code where you'll be ablew to find the path.

Move the existing settings.json file to somewhere safe in case you need to restore it.

You should now be in an empty folder called LocalState.

From a terminal in that folder run `git init` to initialise a repository.

Type `git remote add -t \* -f origin https://github.com/andrewreal/WindowsTerminalOptions.git` to set the remote.

If you get this error - `fatal: invalid refspec '+refs/heads/\*:refs/remotes/origin/\*'` - use the command `git config remote.origin.fetch refs/heads/*:refs/remotes/origin/*`

Run `git fetch`

Run `git checkout master`

Your files should now be in place with the Git repo set up.