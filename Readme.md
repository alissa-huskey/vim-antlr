# vim-antlr

Vim, syntax highlighting for ANTLR versions 3 and 4.

## Installation

#### Pathogen

```sh
cd ~/.vim/bundle && \
git clone https://github.com/dylon/vim-antlr.git
```

See [pathogen.vim] (https://github.com/tpope/vim-pathogen) for more info.

#### Vundle

Add to your `.vimrc`
```vim
Plugin 'mileszs/ack.vim'
```

Then from within vim call `:PluginInstall`

See [Vundle.vim] (https://github.com/VundleVim/Vundle.vim) for more info.

#### NeoBundle

```vim
NeoBundle 'mileszs/ack.vim'
```

See [neobundle.vim] (https://github.com/Shougo/neobundle.vim) for more info.

#### Manual

Download and install the syntax files from the command line:

```sh
mkdir -p "$HOME/.vim/syntax"
curl -LSso "$HOME/.vim/syntax/antlr3.vim" "https://raw.githubusercontent.com/jrozner/vim-antlr/master/syntax/antlr3.vim"
curl -LSso "$HOME/.vim/syntax/antlr4.vim" "https://raw.githubusercontent.com/jrozner/vim-antlr/master/syntax/antlr4.vim"
```

Then add the following to your `.vimrc`:

```vim
au BufRead,BufNewFile *.g set filetype=antlr3
au BufRead,BufNewFile *.g4 set filetype=antlr4
```
