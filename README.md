
## Missing Find Panel Keys (Sublime Text 3 Package)

### Overview

*Missing Find Panel Keys* is a Sublime Text 3 package which provides key bindings for the find panel buttons which are not assigned keys in the default Sublime Text keymap files.

Key bindings added for the Find, Replace, and Incremental Find Panels:

- Toggle Wrap
- Toggle Highlight
- Toggle In Selection

Key bindings added for the Find in Files Panel:

- Toggle Use Buffer
- Toggle Show Context
- Find (ST Build 3132+)
- Replace (ST Build 3132+)

Unfortunately no key binding can be added for the Find in Files panel button, labelled `'...'`, which adds items to the `Where` text box, because there is no command currently available for that action. However users should note that `Tab` can be pressed to focus the `Where` text box at which point its history can be scrolled through using the `Up/Down` keys and deleting its contents will revert it to the default of `Open Files and Folders`.

### Requirements

- Sublime Text 3
- The Find and Replace buttons in the Find in Files panel need version 3132 or later
    - No problem installing on earlier versions but those button's keys won't work

### Installing

Use [Package Control](https://packagecontrol.io/):

- Open the command palette and select: `Package Control: Install Package`
- Wait for the package list to be updated and then select: `Missing Find Panel Keys`
- Note: Package submitted, awaiting addition

Of course users can, if they prefer, [download](https://github.com) the zip file and [install it manually](http://docs.sublimetext.info/en/latest/extensibility/packages.html). There are no package file naming restrictions beyond the usual `.sublime-package` file extension but `MissingFindPanelKeys.sublime-package` would be a sensible choice. Clearly manual installation will prevent Package Control from automatically updating the package.

### Key Bindings

The key bindings are only active when one of the find panels is focused.

Where the first letter of the button's action is already used by another toggle command, the action's last letter is used instead, because that's easy to remember. So `P` is used to toggle `Wrap` since `W` is already used to toggle `Whole Word`, likewise `T` is used to toggle `Show Context` because `C` is already used to toggle `Case Sensitive`.

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
    Find (All)                        Alt+Enter
    Replace (All)                     Ctrl+Alt+Enter
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
    Find (All)                        Alt+Enter
    Replace (All)                     Ctrl+Alt+Enter
    --------------------------------------------------

#### Changing the Keys

If you wish to change the keys all you need do is copy and paste the relevant binding from the keymap file ([Linux](http://github.com), [OSX](http://github.com), [Windows](http://github.com)) into your user keys file.

However, if you don't already know about it, the incredibly useful [PackageResourceViewer](https://packagecontrol.io/packages/PackageResourceViewer) plugin is designed to make these kind of changes with tremendous ease.

### License

This package is licensed under [The MIT License (MIT)](http://github.com).
