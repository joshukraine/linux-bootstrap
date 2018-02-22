Linux Bootstrap
===============

The purpose of this script is to provision a new machine running a fresh install of Ubuntu or other Debian-type Linux system. It includes the software, dotfiles, and general preferences I use for web development. The command line environment is based on Zsh, Vim and Tmux. This setup is intended for a personal development machine, not a web-facing server.

&#9657; **Running macOS? Check out [Mac Bootstrap](http://jsua.co/macos).**

For more Linux bootstrap options, be sure to check out Joshua Steele's [Linux Bootstrap](https://github.com/joshukraine/linux-bootstrap), from which this repo was forked.

Supported distros
-----------------

This script has been successfully tested on the following Linux distros:

* Ubuntu 16.04

Installation
------------

**NOTE: Currently, the installation of Vim is disabled and Vim will need to be [compiled
from source](https://gist.github.com/joshukraine/b9085aeb3dd762cf1d1e1c356974032f) before installing.**

To install with a one-liner, run this:

```sh
bash <(wget -qO- https://raw.githubusercontent.com/speedy1812/linux-bootstrap/master/bootstrap) 2>&1 | tee ~/bootstrap.log
```

Want to read through the script first?

```sh
wget -qO- https://raw.githubusercontent.com/speedy1812/linux-bootstrap/master/bootstrap > bootstrap
less bootstrap
bash bootstrap 2>&1 | tee ~/bootstrap.log
```

What does it do?
----------------

When you invoke `bootstrap`, this is what it does in a nutshell:

* Patch the system and install various software packages.
* Install various software utilities.
* Install [Oh-My-Zsh](https://github.com/robbyrussell/oh-my-zsh).
* Symlink dotfiles to `$HOME`
* Install several fixed-width fonts.
* Install [Vundle](https://github.com/VundleVim/Vundle.vim.git) and plugins for Vim.
* Install [asdf](https://github.com/asdf-vm/asdf).
* Install Ruby, Bundler, and Node.
* Set up Tmux.

License
-------

Copyright (c) 2017 Nathan Day. [MIT License](https://github.com/speedy1812/linux-bootstrap/blob/master/LICENSE)
