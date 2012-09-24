exec-in-window
==============

_exec-in-window_ is replacement for `exec` command used in _Sublime Text 2_ build system

![SublimeText screenshot](https://raw.github.com/vhyza/exec-in-window/master/screenshot.png)

features
--------
* display build results in new _Sublime Text_ window instead of output panel
* execute file without name (unsaved)

installation
------------
go to _Sublime Text_ `Packages` directory

* `~/Library/Application\ Support/Sublime\ Text\ 2/Packages` on _OS X_
* `%APPDATA%/Sublime Text 2/Packages/` on _Windows_
* `~/.config/sublime-text-2/Packages/` on _Linux_

clone repository

    git clone https://github.com/vhyza/exec-in-window.git

usage
-----
* press `Command+B` to build file (unnamed files should have set proper syntax set)
