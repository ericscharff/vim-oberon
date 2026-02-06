# vim-oberon

This repository provides very basic syntax highlighting for the Oberon
programming language.

## Installation

This should be usable with most vim plugin managers. I use
[vim-plug](https://junegunn.github.io/vim-plug/) but others should potentially
work too. This can be installed with something like

```
call plug#begin()
[ ... ]
Plug 'ericscharff/vim-oberon'
call plug#end()
```

## Usage

The syntax highlighting can be enabled by setting the correct file type, e.g.

```
au BufNewFile,BufRead *.Mod set filetype=oberon
au BufNewFile,BufRead *.ob set filetype=oberon
```

