# dotfiles

-   Terminal: [Alacritty](https://github.com/jwilm/alacritty) using zsh w/ [starship prompt](https://starship.rs/) and [color-ls](https://github.com/athityakumar/colorls)
-   Window management: [yabai](https://github.com/koekeishiya/yabai)
-   Hotkeys: [skhd](https://github.com/koekeishiya/skhd)
-   Vim: [neovim](https://neovim.io/) with [Vundle](https://github.com/VundleVim/Vundle.vim) to manage plugins
-   Tools: [tmux](https://github.com/tmux/tmux), [z](https://github.com/rupa/z), [fzf](https://github.com/junegunn/fzf)

## Installation

**Before you get started** make sure you give full disk access permission to your terminal (for writing macos defaults). `System Preferences -> Privacy -> Full Disk Access`.

To install:

`curl -L https://git.io/JeA7g | sh`

This expands to [run.sh](https://github.com/gretzky/dotfiles/blob/master/run.sh) which will fetch this repo and run the install script.

## File overview

-   Configs for the following tools:
    -   Alacritty
    -   fzf
    -   z
    -   git
    -   colorls
    -   skhd
    -   yabai
    -   starship
-   Shell environment configs:
    -   `.zshrc`
    -   `.zlogin.sh`
    -   `.zshenv.sh`
    -   [Antigen]https://github.com/zsh-users/antigen) for zsh plugin management
    -   `.aliases`
    -   `.exports`
-   `Brewfile` (contains all homebrew packages, casks, and mac appstore apps)

The install script will also setup a better Python environment with [pyenv](https://github.com/pyenv/pyenv) and set the global Python version to 3.7 instead of 2 (macOS default).

### Customization

-   The ['highlight color'](https://github.com/gretzky/dotfiles/blob/ad8580a0898c416528cc44e451cc36044d4c299a/macos/.macos#L22-L23) (accent color for mac, typically blue) is set to pink. To set it to a different color:
    -   Pick your desired color and get its RGB value (ex. pink is `255,105,180`)
    -   Take each value and divide it by 255 (ex. pink is now `1, 0.41176470588, 0.70588235294`)
    -   Put them into RGB order (ex. pink is `"1 0.41176470588 0.70588235294"`)

## Acknowledgements

-   [gretzky/dotfiles](https://github.com/gretzky/dotfiles)
