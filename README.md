# exec-in-window

_exec-in-window_ is modified `exec` command used in _Sublime Text 2_ build system

![SublimeText screenshot](https://raw.github.com/vhyza/exec-in-window/master/screenshot.png)

## features

* display build results in new _Sublime Text_ window instead of output panel
* execute *unsaved* files - based on selected syntax

## installation
go to _Sublime Text_ `Packages` directory

* `~/Library/Application\ Support/Sublime\ Text\ 2/Packages` on _OS X_
* `%APPDATA%/Sublime Text 2/Packages/` on _Windows_
* `~/.config/sublime-text-2/Packages/` on _Linux_

clone repository

    git clone https://github.com/vhyza/exec-in-window.git

## usage

modify build settings for desired language

for example for `Ruby` you need to modify file `Packages/Ruby/Ruby.sublime-build` and add line `"target": "exec_in_window"`

whole file should look like this

````json
{
  "cmd": ["/Users/vhyza/.rvm/bin/rvm-auto-ruby", "$file"],
  "target": "exec_in_window",
  "selector": "source.ruby"
}
````

to disable output panel add `"show_panel_on_build": false` into your preferences (`Command+,`)

press `Command+B` to build file (unnamed files should have set proper syntax)
