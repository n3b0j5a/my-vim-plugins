# Vim plugins collection

This is the library of plugins that I use for my daily job. I use it mostly for embedded and kernel
development in C, or C++,  and plugins are chosen according to my needs. I also have my own .vimrc
configuration file which sets a lot of options to vim. Fill free to test it and customize it to your
own needs.

## Plugin details and descrioption

For each plugin, please visit its home page:


* DoxygenToolkit:     https://github.com/vim-scripts/DoxygenToolkit.vim
* a.vim:              https://github.com/vim-scripts/a.vim
* auto-pairs:         https://github.com/jiangmiao/auto-pairs
* cscope-maps:        https://github.com/joe-skb7/cscope-maps.git
* file-line:          https://github.com/bogado/file-line.git
* indentLine:         https://github.com/Yggdroot/indentLine.git
* NERDtree:           https://github.com/scrooloose/nerdtree.git
* supertab:           https://github.com/ervandew/supertab.git
* tagbar:             https://github.com/majutsushi/tagbar.git
* undotree:           https://github.com/mbbill/undotree.git
* vim-airline:        https://github.com/vim-airline/vim-airline
* vim-airline-themes: https://github.com/vim-airline/vim-airline-themes
* vim-gitgutter:      https://github.com/airblade/vim-gitgutter
* vim-plugins:        https://github.com/WolfgangMehner/vim-plugins.git
* vim-repeat:         https://github.com/tpope/vim-repeat
* vim-surround:       https://github.com/tpope/vim-surround
* vim-virtualenv:     https://github.com/plytophogy/vim-virtualenv

## Installation

To install all plugins you should have pathogen installed. Pathogen will
automatically include all plugins from ~/.vim/bundle folder at vim start.
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

## Contributing
Fill free to send suggestions to my mail: chevalierdebalibari@keemail.me

