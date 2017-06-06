
## Missing Find Panel Keys (Sublime Text Package)

### Overview

*Missing Find Panel Keys* is a Sublime Text package which provides key bindings for the find panel toggle buttons which are not assigned keys in the default Sublime Text keymap files.

Key bindings added for the Find, Replace, and Incremental Find Panels:

- Toggle Wrap
- Toggle Highlight
- Toggle In Selection

Key bindings added for the Find in Files Panel:

- Toggle Use Buffer
- Toggle Show Context

Information about the other Find in Files Panel buttons:

- [Dev Build](https://www.sublimetext.com/3dev) 3133 added key bindings for the Find in Files panel `Find` and `Replace` buttons. It is not possible to add key bindings for those buttons to versions earlier than 3133 because no commands existed to perform their actions.
- No key binding can be added for the Find in Files panel button, labelled `'...'`, which adds items to the `Where` text box, because there is no command currently available to launch that action in any version of Sublime Text.
- For mouse-less operation users should note that `Tab` can be pressed to focus the `Where` text box at which point its history can be scrolled through using the `Up/Down` keys and deleting its contents will revert it to its `Open Files and Folders` default.

### Requirements

- Sublime Text version 2 or 3


### Installing

Use [Package Control](https://packagecontrol.io/):

- Open the command palette and select: `Package Control: Install Package`
- Wait for the package list to be updated and then select: `Missing Find Panel Keys`
- Note: Package submitted, awaiting addition

Users can, if they prefer, download the [zip file](https://github.com/mattst/SublimeMissingFindPanelKeys/archive/master.zip) and then [install it manually](http://docs.sublimetext.info/en/latest/extensibility/packages.html). Clearly manual installation will prevent Package Control from automatically updating the package.

### Key Bindings

The key bindings are only active when one of the find panels is focused.

If the first letter of the button's action is already used by another button's command then the action's last letter is used instead because that is easy to remember. i.e.

- `P` is used to toggle `Wrap` since `W` is already used to toggle `Whole Word`
- `T` is used to toggle `Show Context` since `C` is already used to toggle `Case Sensitive`

#### Linux and Windows

    For the Find, Replace, and Incremental Find Panels
    --------------------------------------------------
    Toggle Wrap                       Alt+P
    Toggle In Selection               Alt+S
    Toggle Highlight Matches          Alt+H
    --------------------------------------------------

    For the Find in Files Panel
    --------------------------------------------------
    Toggle Use Buffer                 Alt+B
    Toggle Show Context               Alt+T
    --------------------------------------------------

#### OSX

    For the Find, Replace, and Incremental Find Panels
    --------------------------------------------------
    Toggle Wrap                       Super+Alt+P
    Toggle In Selection               Super+Alt+S
    Toggle Highlight Matches          Super+Alt+H
    --------------------------------------------------

    For the Find in Files Panel
    --------------------------------------------------
    Toggle Use Buffer                 Super+Alt+B
    Toggle Show Context               Super+Alt+T
    --------------------------------------------------

#### Changing the Keys

To change the keys just copy and paste the relevant binding from the keymap file ([Linux](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(Linux).sublime-keymap), [OSX](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(OSX).sublime-keymap), [Windows](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(Windows).sublime-keymap)) into your user keys file and change the key bindings to whatever you want.

Note that the incredibly useful [PackageResourceViewer](https://packagecontrol.io/packages/PackageResourceViewer) plugin is designed to make package changes like this with speed and ease - installing it and learning how to use it will save you a lot of time in the long run.

### License

This package is licensed under [The MIT License (MIT)](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/LICENSE).
