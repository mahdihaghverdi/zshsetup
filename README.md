# Zsh setup of me

## Install Zsh
```
sudo apt install zsh
```

## Install Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install Recommended fonts
[https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)

Note: the fonts are in the repo under /fonts directory

## Install Powerlevel10k
[https://github.com/romkatv/powerlevel10k#installation](https://github.com/romkatv/powerlevel10k#installation)

### Restart zsh
```
exec zsh
```

### Configure the theme
```
p10k configure
```

Note: if didn't work: `$ echo 'source ~/.oh-my-zsh/custom/themes/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc`

## Zsh plugins
1. [Zsh Auto-Suggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh)
    1. clone
    ```
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```

    2. add it:
    ```
        plugins=(
        # other plugins...
        zsh-autosuggestions
    )
    ```

2. [Zsh-Syntax-Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#oh-my-zsh)
    1. clone:
    ```
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```
   
    2. Add it:
    ```
    plugins=( [plugins...] zsh-syntax-highlighting)
    ```
