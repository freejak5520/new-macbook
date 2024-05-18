# New MacBook Setup Guide for Developers

This document summarizes the necessary steps when setting up a new MacBook for development purposes.

## Install Homebrew

Check [brew.sh](https://brew.sh/)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Paste that in a macOS Terminal or Linux shell prompt.

## Install apps

### With brew cask

```
brew install --cask firefox visual-studio-code google-chrome slack iterm2 notion fork bartender postman docker zoom alfred rectangle maccy bitwarden iina textsniper keka appcleaner dbeaver-community synology-drive
```

The apps that can be installed using the command are listed below.

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

### with App Store

- [Dropover](https://apps.apple.com/kr/app/dropover-easier-drag-drop/id1355679052?mt=12)
- [Authy](https://apps.apple.com/kr/app/twilio-authy/id494168017)
- [RunCat](https://apps.apple.com/kr/app/runcat/id1429033973?mt=12)

## Iterm2

### Color Theme

Select and download themes from https://iterm2colorschemes.com/

Double-click the downloaded theme file and apply it to iterm2.

Settings - Profiles - Colors - Color Presets...

### Oh my zsh

https://ohmyz.sh/#install

```
# Install oh-my-zsh via curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install oh-my-zsh via wget
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

### powerlevel10k

https://github.com/romkatv/powerlevel10k

Powerlevel10k is a theme for Zsh. It emphasizes speed, flexibility and out-of-the-box experience.

![powerlevel10k styles](https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/prompt-styles-high-contrast.png)

## Developments

Development environment setup

### Git

https://git-scm.com/

Install and set up a newer version of git using brew instead of the version that comes with Xcode Command Line Tools.

Install git

```
brew install git
```

Add to .zshrc

```
export PATH=/usr/local/bin:$PATH
```

### GitHub CLI

https://cli.github.com/

Install GitHub CLI and log in to GitHub.

Install via brew

```
brew install gh

gh auth login
```

### nvm

https://github.com/nvm-sh/nvm

Install nvm(Node version manager) and install the version of node you want to use.

Install via brew

```
brew install nvm
```

add to .zshrc

```
export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
```

## System Settings

### Remove input source shortcut

Remove the default macOS shortcut to prevent conflicts with Control + Space used in IDEs.

### Trackpad 3 point drag

Set up trackpad 3-point drag.

- Accessibility - Pointer Controls - Trackpad Options
