# Zsh plugins

To enhance your zsh experience and make it more convenient to use, consider adding the following useful plugins

## Oh my zsh

Oh My Zsh is an open source, community-driven framework for managing Zsh configuration, bundled with thousands of helpful functions, helpers, plugins, and themes.

[https://ohmyz.sh/](https://ohmyz.sh/)

```
# Install oh-my-zsh via curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install oh-my-zsh via wget
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

## powerlevel10k

Powerlevel10k is a theme for Zsh. It emphasizes speed, flexibility and out-of-the-box experience.

https://github.com/romkatv/powerlevel10k

![powerlevel10k styles](https://raw.githubusercontent.com/romkatv/powerlevel10k-media/master/prompt-styles-high-contrast.png)

## zsh-autosuggestions

It suggests commands as you type based on history and completions.

[https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md](https://github.com/zsh-users/zsh-autosuggestions)

<a href="https://asciinema.org/a/37390" target="_blank"><img src="https://asciinema.org/a/37390.png" width="400" /></a>

Install command:

```
brew install zsh-autosuggestions
```

To activate the autosuggestions, run the following command to append the content to the end of your .zshrc file:

```shell
echo "source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh"  >> ${ZDOTDIR:-$HOME}/.zshrc
```

Start a new terminal session.

## zsh-autocomplete

A plugin for Zsh that adds real-time type-ahead autocompletion to the command line, similar to desktop apps.

https://github.com/marlonrichert/zsh-autocomplete

Install command:

```
brew install zsh-autocomplete
```

To activate the autocomplete, run the following command to append the content to the end of your .zshrc file:

```shell
echo "source $(brew --prefix)/share/zsh-autocomplete/zsh-autocomplete.plugin.zsh"  >> ${ZDOTDIR:-$HOME}/.zshrc
```

## zsh-syntax-highlighting

A package that provides Fish shell-like syntax highlighting for the Zsh shell.

https://github.com/zsh-users/zsh-syntax-highlighting

Install command:

```shell
brew install zsh-syntax-highlighting
```

To activate the syntax-highlighting, run the following command to append the content to the end of your .zshrc file:

```shell
echo "source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```
