# New macbook check list

## install brew

https://brew.sh/

## install apps

### with Cask

```
brew install --cask firefox visual-studio-code google-chrome slack iterm2 notion fork bartender postman docker zoom alfred rectangle maccy bitwarden iina textsniper keka appcleaner dbeaver-community synology-drive
```

### with App Store

- Dropover
- Authy

## System Settings

### remove input source shortcut

### Trackpad 3 point drag

트랙패드 3포인트 드래그 설정
- 손쉬운 사용 - 포인터 제어기 - 트랙패드 옵션

## Iterm2

### Color Theme

https://iterm2colorschemes.com/

테마 선택 및 다운로드

더블클릭해 iterm2에 적용

Settings - Profiles - Colors - Color Presets...

### Oh my zsh

https://ohmyz.sh/#install

### Power Level 10k

https://github.com/romkatv/powerlevel10k 

## Developments

### Git

Install git

```
brew install git
```

add to .zshrc
```
export PATH=/usr/local/bin:$PATH
```

### Gitbuh cli

```
brew install gh

gh auth login
```

### nvm

Install

```
brew install nvm
```

add to .zshrc

```
export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
```

