# New MacBook Setup Guide for Me

This document summarizes the necessary steps when setting up a new MacBook for development purposes.

## Install Homebrew

[https://brew.sh/](https://brew.sh/)

To install Homebrew on macOS or Linux, open a terminal and paste the following command:

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Install apps

### With brew

```shell
brew install --cask firefox visual-studio-code google-chrome slack iterm2 notion fork bartender postman docker zoom alfred rectangle maccy bitwarden iina textsniper keka appcleaner dbeaver-community synology-drive
```

The following apps can be installed using the above command:

- Firefox - Web browser
- Google Chrome - Web browser
- Visual Studio Code - Code editor
- Slack - Team communication tool
- Zoom - Video conferencing tool
- Notion - Project management and collaboration tool
- Fork - Git client
- Postman - API development and testing tool
- Docker - Container platform
- DBeaver Community - Database management tool
- Alfred - Productivity app
- Rectangle - Window management tool
- Maccy - Clipboard manager
- Bitwarden - Password manager
- iTerm2 - Terminal emulator
- Bartender - Menu bar icon manager
- IINA - Video player
- TextSniper - OCR tool
- Keka - Compression/decompression tool
- AppCleaner - App removal tool
- Synology Drive - File synchronization tool

#### Stats

https://github.com/exelban/stats

To install it using Homebrew, open the Terminal app and type:

```shell
brew install stats
```

### with App Store

- [Dropover](https://apps.apple.com/kr/app/dropover-easier-drag-drop/id1355679052?mt=12)
- [Authy](https://apps.apple.com/kr/app/twilio-authy/id494168017)
- [RunCat](https://apps.apple.com/kr/app/runcat/id1429033973?mt=12)

## Iterm2

### Color Theme

Select and download themes from https://iterm2colorschemes.com/

Double-click the downloaded theme file and apply it to iterm2.

Settings -> Profiles -> Colors -> Color Presets...

## Zsh plugins

Check [Zsh plugins](./zsh-plugins.md)

## Developments

Development environment setup

### Git

https://git-scm.com/

Install and set up a newer version of git using brew instead of the version that comes with Xcode Command Line Tools.

Install git

```shell
brew install git
```

Add to .zshrc

```shell
export PATH=/usr/local/bin:$PATH
```

#### Set default editor VSCode

```shell
git config --global core.editor "code --wait"
```

#### Set default difftool VSCode

```shell
git config --global -e
```

Add to .gitconfig

```ini
[diff]
    tool = default-difftool
[difftool "default-difftool"]
    cmd = code --wait --diff $LOCAL $REMOTE
```

#### Set default mergetool

```shell
git config --global -e
```

Add to .gitconfig

```ini
[merge]
    tool = vscode
[mergetool "vscode"]
    cmd = code --wait $MERGED
```

### GitHub CLI

https://cli.github.com/

Install GitHub CLI and log in to GitHub.

Install via brew

```shell
brew install gh

gh auth login
```

### nvm

https://github.com/nvm-sh/nvm

Install nvm(Node version manager) and install the version of node you want to use.

Install via brew

```shell
brew install nvm
```

add to .zshrc

```shell
export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
```

## System Settings

### Remove input source shortcut

Remove the default macOS shortcut to prevent conflicts with Control + Space used in IDEs.

### Trackpad 3 point drag

Set up trackpad 3-point drag.

- Accessibility -> Pointer Controls -> Trackpad Options
