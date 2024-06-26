# Neovim

The
[janet-neovim-trial-kit](https://github.com/sogaiu/janet-neovim-trial-kit)
may be a simple way to get a taste of what's possible without having
to gather a bunch of packages and perform a lot of configuration
upfront.

Below are some specific plugins that provide a variety of features
related to Janet for Neovim.  The trial kit mentioned above makes use
of the plugins below so examining the kit might give some hints about
how to configure your own setup.

## Indentation

Indentation features can be had via
[janet.vim](https://github.com/janet-lang/janet.vim).

### janet.vim

Apart from indentation, syntax highlighting is also provided, though
for the latter, using nvim-treesitter (see below) is another option.

## Syntax Highlighting

Although janet.vim provides syntax highlighting, an alternative is to
use
[nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter/).

### nvim-treesitter

The Janet support in nvim-treesitter is limited to syntax highlighting.

## REPL Interaction

Interaction via REPL is available via
[conjure](https://github.com/Olical/conjure/).

### conjure

There are two ways to interact via REPL using conjure:

* netrepl REPL
* stdio-based REPL

## Linting

One way to get some linting of Janet code is via
[nvim-lint](https://github.com/mfussenegger/nvim-lint).

### nvim-lint

There is built-in support for Janet in nvim-lint.

