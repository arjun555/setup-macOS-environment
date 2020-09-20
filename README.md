# setup-web-environment
Sets for setting up your macOS environment for web development

## Command Line Tools
### Homebrew
Homebrew is a package manager. Once Homebrew is installed, we can use it to install our other tools.

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

### iTerm2
iTerm2 is a replacement terminal for mac. Amongst other features, it has better auto-complete - which is why I like it

`brew cask install iTerm2`

### Git
Version control.

`brew install git`

### Zsh
Z Shell is an extended version of the Bourne Shell. It has a lot of features, themes and plugin support. I find the Tab auto-completion of paths and recursive path  really useful in day-to-day coding.

`brew install zsh`

Configurations for zsh are stored in the `.zshrc` file. Once changes are made, you need to reload by running:

`source ~/.zshrc`

### Oh-my-zsh
Oh-my-zsh is a framework for Zsh. Comes with a bunch of features and plugin support.

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

If `zsh` is not set to your default shell, run the following:

`chsh -s $(which zsh)`

### SSH Key
SSH Keys can be used to establish a secure connection with the Github servers. This allows you to clone, pull, push, etc. without having to enter in your github email and password each time.
To generate a new SSH Key, run:

`ssh-keygen -t rsa -C "your_email@example.com"`

If your .ssh directory does not exisit, it will generate this for you along with your public and private keys. 

### NVM (Node Version Manager)
NVM is a version manager for Node.js

`brew install nvm`

To download and install the latest version of Node.js, run:

`nvm install node`

### asdf
Version manager that I use to control Elixir/Erlang. It allows you to config a file `.tool-versions` within your application, to ensure you have the right version installed.

`brew install asdf`

### Docker
Docker allows you to package your code and all it's dependancies, then run it in an isolated environment called containers.

`brew cask install docker`

### Tableplus
GUI for databases

`brew cask install tableplus`
