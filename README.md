# Linux Bootstrap

The purpose of this script is to provision a new machine running a fresh install of Ubuntu or other Debian-type Linux system. It includes the software, dotfiles, and general preference I use for web development. The command line environment is based on zsh, vim and tmux. This setup is intended for a personal development machine, not a web-facing server.

&#9657; **Running OS X? Check out [Mac Bootstrap](https://github.com/joshukraine/mac-bootstrap).**

### Supported distros

This script has been successfully tested on the following Linux distros:

* Ubuntu 14.04, 15.04
* Lubuntu 14.10, 15.04
* Debian 7.8, 8.2

### Installation

To install with a one-liner, run this:

```sh
bash <(wget -qO- https://raw.githubusercontent.com/joshukraine/dotfiles/linux-bootstrap/bootstrap) 2>&1 | tee ~/bootstrap.log
```

Want to read through the script first?

```sh
wget -qO- https://raw.githubusercontent.com/joshukraine/dotfiles/linux-bootstrap/bootstrap > bootstrap
less bootstrap
bash bootstrap 2>&1 | tee ~/bootstrap.log
```

### What does it do?

When you invoke `bootstrap`, this is what it does in a nutshell:

* Patch the system and install various software packages
* Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
* Symlink dotfiles to `$HOME`
* Install several fixed-width fonts.
* Install Vundle and plugins for vim.
* Install [rbenv](https://github.com/sstephenson/rbenv) and [ruby-build](https://github.com/sstephenson/ruby-build#readme)
* Install Ruby, Rails and related packages
* Install Google Chrome (for compatible distros)


### Some of my favorite dotfile repos

* Pro Vim (https://github.com/Integralist/ProVim)
* Trevor Brown (https://github.com/Stratus3D/dotfiles)
* Lars Kappert (https://github.com/webpro/dotfiles)
* Ryan Bates (https://github.com/ryanb/dotfiles)
* thoughtbot (https://github.com/thoughtbot/dotfiles)
* Ben Orenstein (https://github.com/r00k/dotfiles)
* Joshua Clayton (https://github.com/joshuaclayton/dotfiles)
* Drew Neil (https://github.com/nelstrom/dotfiles)
* Chris Toomey (https://github.com/christoomey/dotfiles)
* Kevin Suttle (https://github.com/kevinSuttle/OSXDefaults)
* Carlos Becker (https://github.com/caarlos0/dotfiles)
* Zach Holman (https://github.com/holman/dotfiles/)
* Mathias Bynens (https://github.com/mathiasbynens/dotfiles/)
* Paul Irish (https://github.com/paulirish/dotfiles)


### Helpful web resources on dotfiles, et al.

* http://dotfiles.github.io/
* https://medium.com/@webprolific/getting-started-with-dotfiles-43c3602fd789
* http://code.tutsplus.com/tutorials/setting-up-a-mac-dev-machine-from-zero-to-hero-with-dotfiles--net-35449
* https://github.com/webpro/awesome-dotfiles
* http://blog.smalleycreative.com/tutorials/using-git-and-github-to-manage-your-dotfiles/
* http://carlosbecker.com/posts/first-steps-with-mac-os-x-as-a-developer/
* https://mattstauffer.co/blog/setting-up-a-new-os-x-development-machine-part-1-core-files-and-custom-shell
* http://blog.smalleycreative.com/tutorials/using-git-and-github-to-manage-your-dotfiles/
