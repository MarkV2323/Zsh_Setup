# Zsh and Oh My Zsh


### What are they?
- Zsh is a shell, specifically an extension of bash that provides more functionality than bash.
- Oh My Zsh is a configuration manager framework for Zsh, to make using Zsh a bit more enjoyble allowing for the additions of plugins and themes for the shell.

### Differences from Bash
One primary difference between the two are the way configuration files are read.

Bash reads in from the following config files,
- .bashrc (non login interactive shells)
- .profile (login shells)
- .bash_profile (login shells)
- .inputrc

Zsh reads in from the following config files,
- .zshrc (all interactive shells)
- .zprofile (login shells)

Most configurations between the two are not compatible and required porting, usually from bash over to zsh. Major scripting differences between the two also exist and it's worth reading up on if complex scripts are being ran.

You can find more information at the following stack exchange link,
[Link Here](https://apple.stackexchange.com/questions/361870/what-are-the-practical-differences-between-bash-and-zsh)

### Installtion of Zsh
Zsh is the default shell for Mac OS X and Kali Linux, hence does not need to be installed for those Operating Systems.

You can install Zsh from primary package repos for most linux system, it's reccomended to update your packges first though.
```
sudo apt update
```
```
sudo apt install zsh
```
Now to make Zsh the default shell for the system, run the following command,
```
chsh -s $(which zsh)
```
Zsh is now installed and the default shell for the terminal to launch.

### Installtion of Oh My Zsh
*Ensure Zsh is already installed prior to install Oh My Zsh*

You can install Oh My Zsh in three ways via three different command line tools,
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```
sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
Oh My Zsh will now be installed on your system. You can find more detailed instructions on the [Oh My Zsh github repo](https://github.com/ohmyzsh/ohmyzsh) if need be.

### Configuration of Oh My Zsh
As mentioned earlier, you can edit the configuration file,

```
vi ~/.zshrc
```

This GitHub Repo should contain my favorite general settings for Oh My Zsh so you can just copy and paste those into that file. For more detailed information on plugins and themes, check out the [Oh My Zsh github repo](https://github.com/ohmyzsh/ohmyzsh) if need be.
