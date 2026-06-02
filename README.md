# vim-oberon

This repository provides very basic syntax highlighting for the Oberon
programming language.

# Installation

This should be usable with most vim/nvim plugin managers. I use
[vim-plug](https://junegunn.github.io/vim-plug/) but others should probably
work too. This can be installed with something like

```
call plug#begin()
[ ... ]
Plug 'ericscharff/vim-oberon'
call plug#end()
```

With nvim builtin vim-pack, this can be
```
vim.pack.add({
  'https://github.com/ericscharff/vim-oberon',
})
```

Or, for lazy.vim, it can be configured with

```
{
  "ericscharff/vim-oberon",
  ft = "oberon"
}
```

# Usage

The syntax highlighting can be enabled by setting the correct file type, e.g.

```
au BufNewFile,BufRead *.Mod set filetype=oberon
au BufNewFile,BufRead *.ob set filetype=oberon
```

Or for neovim `init.lua`:

```
vim.filetype.add({
  extension = {
    ob = 'oberon',
  },
})
```

# Related Projects

I use this for synatx highlighting for
[my Oberon compiler](https://github.com/ericscharff/oberon-compiler) which is a
self-hosting Oberon compiler.
