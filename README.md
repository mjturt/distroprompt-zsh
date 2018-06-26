# distroprompt-zsh
Minimal ZSH prompt that shows current OS icon. No other external dependencies (like oh-my-zsh) needed than [Nerd fonts patched font](https://github.com/ryanoasis/nerd-fonts). Based on [karu-prompt by zaari](https://gitlab.com/timosaarinen/karu).
* On left side only OS-icon and arrow that turns red if last command fails (returns other that 0)
* On right current directory if its not current users home
* Git status on right (branch, clean, dirty, ahead, behind)
* OS icon turns to hashtag if root
* OS icon turns to red lock if user does not have write permission to current directory

Supported operating systems are some of most used Linux distros (see below), FreeBSD and MacOS.

If distro is not supported but still Linux it shows Tux-icon.

![distroprompt](/screenshots/distroprompt.png)

Some of the supported OSs

![distroprompt distros](/screenshots/distroprompt-distros.png)

## Full list of supported OSs
* Linux: Gentoo, Arch, Manjaro, Debian, Ubuntu, Raspbian, Mint, Devuan, Slackware, SuSE, RHEL, Fedora, CentOS, NixOS, Elementary, Alpine, Mageia, Sabayon
* FreeBSD
* MacOS

## Install
First install some font from [Nerd Fonts](https://nerdfonts.com) and make sure your terminal uses it.

Then just copy distroprompt.zsh somewhere like ~/.zsh/themes and source it from your ~/.zshrc

For example:
```
git clone https://github.com/mjturt/distroprompt-zsh.git
cd distroprompt-zsh
mkdir -p ~/.zsh/themes
cp distroprompt.zsh ~/.zsh/themes
echo "source ~/.zsh/themes/distroprompt.zsh" >> ~/.zshrc
```
