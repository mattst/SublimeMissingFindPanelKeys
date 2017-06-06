
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
- Wait for the package list to be updated and then select: `MissingFindPanelKeys`
- Note: Package submitted, awaiting addition

Users can, if they prefer, download the [zip file](https://github.com/mattst/SublimeMissingFindPanelKeys/archive/master.zip) and then [install it manually](http://docs.sublimetext.info/en/latest/extensibility/packages.html); `MissingFindPanelKeys.sublime-package` should be used as the installed package file name or, if unzipping for folder installation, then `MissingFindPanelKeys` should be used as the folder name.

### Key Bindings

The key bindings are only active when one of the find panels is focused.

If the first letter of the button's action can not be used for the key binding then the action's last letter is used instead because that is easy to remember. The following key bindings use the last letter instead of the first:

- `P` is used to toggle `Wrap` since `W` is already used by `toggle_whole_word`
- `T` is used to toggle `Show Context` since `C` is already used by `toggle_case_sensitive`
- OSX Only: `N` is used to toggle `In Selection` since `S` is used by `save_all` (which must remain active)

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
    Toggle In Selection               Super+Alt+N
    Toggle Highlight Matches          Super+Alt+H
    --------------------------------------------------

    For the Find in Files Panel
    --------------------------------------------------
    Toggle Use Buffer                 Super+Alt+B
    Toggle Show Context               Super+Alt+T
    --------------------------------------------------

#### Changing the Keys

To change the keys just copy and paste the relevant binding from the default keymap file, `Menu --> Preferences --> Package Settings --> MissingFindPanelKeys --> Key Bindings - Default` / GitHub links [Linux](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(Linux).sublime-keymap), [OSX](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(OSX).sublime-keymap), [Windows](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/Default%20(Windows).sublime-keymap), into your user keys file and change the keys to whatever you want.

Note that the [PackageResourceViewer](https://packagecontrol.io/packages/PackageResourceViewer) plugin allows package changes to be made with speed and ease, installing and learning how to use it saves a lot of time in the long run.

### License

This package is licensed under [The MIT License (MIT)](https://github.com/mattst/SublimeMissingFindPanelKeys/blob/master/LICENSE).
