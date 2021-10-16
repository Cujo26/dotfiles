# Cujo's Dotfiles

Literally just my dotfiles. Currently using package names from the Arch repos and AUR.

Managed with Chezmoi

## Applications used:

* Vim
* Zsh
* Sway (WIP)
* Mpv
* Alacritty
* brightnessctl
* networkmanager
* newsboat
* qutebrowser
* i3-swallow

## Deployment Steps:

On the destination  machine, initialize chezmoi with your dotfiles repo:

    chezmoi init https://github.com/username/dotfiles.git

This will check out the repo and any submodules and optionally create a chezmoi
config file for you. It won't make any changes to your home directory until you
run:

    chezmoi apply

If your dotfiles repo is `https://github.com/username/dotfiles.git` then the
above two commands can be combined into just:

    chezmoi init --apply username

On any machine, you can pull and apply the latest changes from your repo with:

    chezmoi update

For a full list of commands run:

    chezmoi help
