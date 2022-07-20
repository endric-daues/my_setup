# Setting up my Development Environment

## Hardware

I work on a MacBook Air (M2, 2022) with 16GB of RAM. 

## Installations

### Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### ITerm2
```
brew install --cask iterm2
```

### oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Install the following plug-ins:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

Run the following two commands in your terminal to install a nice color scheme, and import this in iTerm2 -> Preferences -> Profiles -> Colors -> Color Presets -> Import...
```
$ cd Downloads
$ curl -O https://raw.githubusercontent.com/MartinSeeler/iterm2-material-design/master/material-design-colors.itermcolors
```

### Powerlevel10k

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

To configure this theme simply run `p10k configure` in your terminal.

### Configuration

I configure my `~/.zshrc` as shown in the file. This is where you'll see the plug-ins I am using. I also included my `.p10k.zsh` file for reference.

