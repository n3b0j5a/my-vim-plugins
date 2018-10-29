# Vim plugins collection 

This is the library of plugins that I use for my daily job. 

## Plugins description
Library currently has following plugins 
* Conque-GDB 
* Conque-Shell
* DoxygenToolkit
* a.vim
* auto-pairs
* indentLine
* nerdtree
* supertab
* syntastic
* undotree
* vim-plugins
* vim-repeat
* vim-sorround


## Installation

To install all plugins you should have pathogen installed. Pathogen will
automaticaly include all plugins from ~/.vim/bunde folder at vim start.
To install pathogen run following commands:

```
mkdir -p ~/.vim/autoload ~/.vim/bundle && \
curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim
echo 'execute pathogen#infect()' >> ~/.vimrc
```
Next, clone this repository into bundle folder:

```
cd ~/.vim/bundle
git clone git@github.com:ChevalierDeBalibari/my-vim-plugins.git
git submodule init
```

That's all!

## Additional information

This repository contains only a portion of my complete vim installation that includes:

* Collection of vim plugins
* Optional patches for some plugins
* Collection of vim themes
* Custom .vimrc file
* Script for automatic installation of all above mentioned stuff

## Conttributing
please have a look at [CONTRIBUTING.md](CONTRIBUTING.md)

