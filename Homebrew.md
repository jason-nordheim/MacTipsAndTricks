
# Getting started with Homebrew 
## Install 
If you haven't already installed the xCode tools, you will need to do so: 
```bash
➜ xcode-select --install 
```
Next you can proceed to installing homebrew using the following command:
```bash
➜ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
You should then be prompted to press `RETURN` to continue, and then be prompted again, but this time for your admistrator password.
> As you type, you will not see anything appear in the password field; note that terminal is capturing your input, it just does not display in the window. 


## Brew Utilities 

### Cask
There are a lot of application for Mac that are not on the Mac App Store. `Cask` is a CLI package manager, that allows you to find, download, install, uninstall, and update numerous Mac applications very easily.

### Cask Installation
With homebrew installed, simply type: 
```zsh
➜ brew install cask 
```

### Cask Basics 
Finding Applications and Packages 
```zsh
# List all of them, like this, 
➜ brew search --casks # will return all the casks (there are TONS!!!)
➜ brew search discord # will search for an app or package named 'discord' and display the result 

# Terminal output will look somoething like: 
# ==> Casks
# discord                                           homebrew/cask-versions/discord-ptb 
```
when you have found an applciation that you would like to install, you can do so in the following manner: 
```zsh 
➜ brew cask install discord # this will try to install a cask named 'discord' 
```
Why is this awesome: 
* It downloads the ISO/DMG for you
* You do **not** have to go through an instal wizard. 
* There are no files to clean-up after install. 
* Brew `cask` can keep the application up-to-date for you. 

So how do you update? 
```zsh 
➜ brew cask upgrade # this will upgrade every application that was installed using cask 
```

#### Accessing help documentation 
```zsh 
➜ brew cask help
#=> Homebrew Cask provides a friendly CLI workflow for the administration
#=> of macOS applications distributed as binaries.
#=>
#=> Commands:
#=> 
#=>     --cache    display the file used to cache the Cask
#=>     audit      verifies installability of Casks
#=>     cat        dump raw source of the given Cask to the standard output
#=>     create     creates the given Cask and opens it in an editor
#=>     doctor     checks for configuration issues
#=>     edit       edits the given Cask
#=>     fetch      downloads remote application files to local cache
#=>     home       opens the homepage of the given Cask
#=>     info       displays information about the given Cask
#=>     install    installs the given Cask
#=>     list       with no args, lists installed Casks; given installed Casks, lists staged files
#=>     outdated   list the outdated installed Casks
#=>     reinstall  reinstalls the given Cask
#=>     style      checks Cask style using RuboCop
#=>     uninstall  uninstalls the given Cask
#=>     upgrade    upgrades all outdated casks
#=>     zap        zaps all files associated with the given Cask
#=> 
# See also "man brew-cask"
```

### HTOP 
