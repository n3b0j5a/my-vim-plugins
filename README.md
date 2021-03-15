# Vim plugins collection

This is the library of plugins that I use for my daily job. I use it mostly for embedded and kernel
development in C, or C++,  and plugins are chosen according to my needs. I also have my own .vimrc
configuration file which sets a lot of options to vim. Fill free to test it and customize it to your
own needs.

## Plugin details and description

For each plugin, please visit its home page:

* Conque-GDB:               https://github.com/vim-scripts/Conque-GDB.git
* DoxygenToolkit.vim:       https://github.com/vim-scripts/DoxygenToolkit.vim.git
* a.vim:                    https://github.com/vim-scripts/a.vim.git
* auto-pairs:               https://github.com/vim-scripts/auto-pairs.git
* cscope-maps:              https://github.com/joe-skb7/cscope-maps.git
* file-line:                https://github.com/bogado/file-line.git
* indentLine:               https://github.com/Yggdroot/indentLine.git
* nerdtree:                 https://github.com/scrooloose/nerdtree.git
* space-vim-dark:           https://github.com/liuchengxu/space-vim-dark.git
* supertab:                 https://github.com/vim-scripts/supertab.git
* tagbar:                   https://github.com/majutsushi/tagbar.git
* undotree:                 https://github.com/mbbill/undotree.git
* vim-airline:              https://github.com/vim-airline/vim-airline.git
* vim-airline-themes:       https://github.com/vim-airline/vim-airline-themes.git
* vim-better-whitespace:    https://github.com/ntpeters/vim-better-whitespace.git
* vim-gitgutter:            https://github.com/airblade/vim-gitgutter
* vim-instant-markdown:     https://github.com/suan/vim-instant-markdown
* vim-linux-coding-style:   https://github.com/vivien/vim-linux-coding-style
* vim-plugins:              https://github.com/WolfgangMehner/vim-plugins.git
* vim-repeat:               https://github.com/tpope/vim-repeat
* vim-surround:             https://github.com/tpope/vim-surround.git
* vim-virtualenv:           https://github.com/plytophogy/vim-virtualenv.git
* vimagit:                  https://github.com/jreybert/vimagit.git

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
git clone --recursive https://github.com/ChevalierDeBalibari/my-vim-plugins.git .
```

That's all!

## Fix a.vim shortcut conflict

Apply following patch to a.vim plugin:

```
diff --git a/plugin/a.vim b/plugin/a.vim
index 637feb5..deb5d77 100644
--- a/plugin/a.vim
+++ b/plugin/a.vim
@@ -559,8 +559,8 @@ comm! -nargs=? -bang IHT call AlternateOpenFileUnderCursor("t<bang>", <f-args>)
 comm! -nargs=? -bang IHN call AlternateOpenNextFile("<bang>")
 imap <Leader>ih <ESC>:IHS<CR>
 nmap <Leader>ih :IHS<CR>
-imap <Leader>is <ESC>:IHS<CR>:A<CR>
-nmap <Leader>is :IHS<CR>:A<CR>
+imap <Leader>ia <ESC>:IHS<CR>:A<CR>
+nmap <Leader>ia :IHS<CR>:A<CR>
 imap <Leader>ihn <ESC>:IHN<CR>
 nmap <Leader>ihn :IHN<CR>

```

## Additional information

This repository contains only a portion of my complete vim installation that includes:

* Collection of vim plugins
* Optional patches for some plugins
* Collection of vim themes
* Custom .vimrc file
* Script for automatic installation of all above mentioned stuff

## Contributing
Send all suggestions to my mail: nebojsa@keemail.me

