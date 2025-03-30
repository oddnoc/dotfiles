# Chezmoi dotfiles

## Installation steps

1. Install chezmoi & git-lite

    ```sh
    doas pkg install chezmoi git-lite
    ```

1. Install [Oh My Zsh](https://ohmyz.sh)
1. Install powerlevel10k

    ```sh
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
    ```

1. Install and apply these dotfiles

    ```sh
    chezmoi init -a https://github.com/oddnoc/dotfiles.git
    ```

1. Restart ZSH

    ```sh
    exec zsh
    ```
