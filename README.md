[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# zsh-kali
zsh configuration adapted for macos based on [Kali Linux](https://kali.org) [2020.3 release](https://www.kali.org/news/kali-2020-3-release/)

<img width="670" alt="Screenshot 2023-03-06 at 1 12 55 PM" src="https://user-images.githubusercontent.com/39002684/223195389-7af66517-f8e6-4918-8470-13ca027e85ca.png">


This .zshrc file uses a similar config as Kali Linux, but also includes git status with the prompt. [Read about the customizations He made.](https://statropy.com/blog/kali-linux-zsh-for-macos/)

## Install

Install the [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting), [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

```
sudo apt/<whatever pkg manager> install zsh-syntax-highlighting zsh-autosuggestions
```

Backup the existing `.zshrc` and symlink the .zshrc file from this repo to your home directory.

```
git clone https://github.com/Deemocean/zsh-kali.git
mv ~/.zshrc ~/.zshrc.orig
ln -s <absolute-path-to-your-git-clone-dir>/.zshrc ~/.zshrc
```

In the Terminal Preferences for the selected Profile, change the font to `JetBrain Mono`. Quit and restart Terminal.

To add your own alias or other commands without having to edit `.zshrc`, create a `.alias` file in the home directory. The `.zshrc` file will load it if it exists.


# Use ZSH as the default shell

```
chsh -s $(which zsh)
```

# Make Ctrl Z the intr key

```
stty intr ^z
```
