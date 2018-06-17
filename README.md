# distroprompt-zsh
Minimal ZSH prompt that shows current OS icon. No other external dependencies (like oh-my-zsh) than [Nerd fonts patched font](https://github.com/ryanoasis/nerd-fonts). Based on [karu-prompt by zaari](https://gitlab.com/timosaarinen/karu).
* On left side only OS-icon and arrow that turns red if last command fails (returns other that 0)
* On right current directory if its not current users home
* Git status on right (branch, clean, dirty, ahead, behind)
* OS icon turns to hashtag if root
* OS icon turns to red lock if current user does not have permissions to write

Supported operating systems are some of most used Linux distros (if cant find icon for distro, shows tux-icon), FreeBSD and MacOS.

![distroprompt](/screenshots/distroprompt.png)

Some other distros and MacOS:

![distroprompt distros](/screenshots/distroprompt-distros.png)

## Install
Just copy distroprompt.zsh somewhere like ~/.zsh/themes and source it from your ~/.zshrc

For example:
```
git clone https://github.com/mjturt/distroprompt-zsh.git
cd distroprompt-zsh
mkdir -p ~/.zsh/themes
cp distroprompt.zsh ~/.zsh/themes
echo "source ~/.zsh/themes/distroprompt.zsh" >> ~/.zshrc
```
