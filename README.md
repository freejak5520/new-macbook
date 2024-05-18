# New macbook check list

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

### with App Store

- [Dropover](https://apps.apple.com/kr/app/dropover-easier-drag-drop/id1355679052?mt=12)
- [Authy](https://apps.apple.com/kr/app/twilio-authy/id494168017)
- [RunCat](https://apps.apple.com/kr/app/runcat/id1429033973?mt=12)

## Iterm2

### Color Theme

https://iterm2colorschemes.com/ 에서 테마 선택 및 다운로드

다운로드한 테마 파일을 더블클릭해 iterm2에 적용

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

개발 환경 설정

### Git

https://git-scm.com/

Xcode Command Line Tools 에 같이 설치되는 Git 버전보다 최신 버전을 사용하기 위해 brew를 이용해 git을 설치하고 설정합니다.

Install git

```
brew install git
```

add to .zshrc

```
export PATH=/usr/local/bin:$PATH
```

### GitHub CLI

https://cli.github.com/

GitHub CLI를 설치하고 GitHub에 로그인합니다.

Install via brew

```
brew install gh

gh auth login
```

### nvm

https://github.com/nvm-sh/nvm

Node version manager 를 설치하고 사용할 node 버전을 설치합니다.

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

IDE에서 사용하는 Control + Space 와 충돌 방지를 위해 맥 기본 단축키 제거

### Trackpad 3 point drag

트랙패드 3포인트 드래그 설정

- 손쉬운 사용 - 포인터 제어기 - 트랙패드 옵션
