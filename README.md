# Dotfiles

To-Do: write install script

## Software

## emacs
use yay to install newest emacs

git clone --depth 1 https://github.com/hlissner/doom-emacs ~/.emacs.d

~/.emacs.d/bin/doom install

### zsh

install with package manager if not installed.

chsh -s $(which zsh)

### oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

### Sauce Code Font (Nerd Fonts)

yay Nerd Fonts Source Code Pro Complete

alternatively:
git clone https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/SourceCodePro/Regular/complete ~/nerdfonts

For system wide installation, copy the fonts to /usr/share/fonts and run sudo fc-cache to rebuild the font cache, 

or for user local installation, make sure ~/.fonts exists, copy them into there, then rebuild the font cache.

### bat, fd, vivid

install with package manager if not installed.

check bat-extras https://github.com/eth-p/bat-extras/blob/master/README.md#installation

### tmux, tilix

install with package manager if not installed.

tilix needs to be added to $mod+return in i3 config

### samba

install with package manager if not installed.

smbclient

smbclient requires a /etc/samba/smb.conf file (see #Installation), which you can create as an empty file using the touch utility.

reboot



