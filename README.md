1> Download WM file
https://www.linuxvmimages.com/images/ubuntu-2004

Username: ubuntu
Password : ubuntu

Change network to NAT (support SSH)
ssh TCP 127.0.0.1 2222
        10.0.15.2 22 
		
Enable SSH
https://linuxconfig.org/enable-ssh-on-ubuntu-20-04-focal-fossa-linux
sudo apt install ssh
sudo systemctl enable --now ssh
		
2> Change password
sudo passwd ubuntu

3> ZSH
sudo apt-get update
sudo apt install curl zsh git tmux autojump ranger kitty

https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH
sudo apt install zsh
Make it your default shell: chsh -s $(which zsh)

https://github.com/ohmyzsh/ohmyzsh
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

https://github.com/zsh-users

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions

git clone https://github.com/zsh-users/zsh-history-substring-search ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-history-substring-search

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

https://github.com/ogham/exa

https://github.com/sharkdp/fd

Neovim
https://github.com/ChristianChiarulli/LunarVim

NerdFont
sudo mkdir ${HOME}/.local/share/fonts/

https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/FiraCode/Retina/complete/Fira%20Code%20Retina%20Nerd%20Font%20Complete.ttf

sudo fc-cache -f

fonts fc-list | grep "Fira"

fzf
https://github.com/junegunn/fzf

git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install

tmux TPM
https://github.com/tmux-plugins/tpm

Ranger 
~/.config/ranger

