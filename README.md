# 'Open in' buttons for macOS Finder toolbar

Works on macOS Mojave.

![screenshot](src/images/screenshot.png "screenshot")

## Available apps

- Terminal
- iTerm
- Visual Studio Code
- Sublime text

## How to
- Download apps
- Copy to Applications folder
- and drag it to Finder toolbar (hold `⌘cmd`)

## Sublime Text
Run the following command to add a command line shortcut for Sublime Text. This is needed for the Finder button to work.

```bash
# Sublime Text 2
# ln -s /Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl /usr/local/bin/sublime

# Sublime Text 3
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

## Visual Studio Code
Run the following command in Visual Studio Code (`Cmd + Shift + P`)

```
>Shell Command: Install 'code' command in PATH
```

Issues: Does not open the current folder when buttons are clicked without selecting a file/folder. It should open the current folder if no file/folder is selected.