# Emacs

## Basic Language Support

There are at least two major modes providing Janet support:

* [janet-mode](https://github.com/ALSchwalm/janet-mode/)
* [janet-ts-mode](https://github.com/sogaiu/janet-ts-mode)

Neither mode comes with built-in REPL support.  See further down for
some options.

Note that if you're using an Emacs with the native tree-sitter
integration, the
[janet-emacs-trial-kit](https://github.com/sogaiu/janet-emacs-trial-kit)
may be a simple way to get a taste of what's possible without having
to gather a bunch of packages and perform a lot of configuration
upfront.

If you're a Spacemacs user, you might find
[spacemacs-janet-layer](https://github.com/5thWall/spacemacs-janet-layer)
to be of interest.

### janet-mode

This major mode provides at least:

* Syntax highlighting
* Indentation
* Imenu

If some bits don't quite work, it might be worth checking out the
issues, PRs, and/or forks.

### janet-ts-mode

This major mode relies on the integrated tree-sitter support in Emacs
\>= 29.  Its features include at least:

* Syntax highlighting
* Indentation
* Imenu
* Which-function support
* Structural navigation

In addition, there are some experimental features which can be enabled.

## REPL Support

There are two types of REPL support available, stdio-based and
netrepl-based.

### Stdio-based REPL

There are at least four implementations of stdio-based REPL
connections:

* [ajrepl](https://github.com/sogaiu/ajrepl)
* [ijanet-mode](https://github.com/SerialDev/ijanet-mode)
* [inf-janet](https://github.com/velkyel/inf-janet)
* [inf-janet](https://github.com/mpwillson/emacs/blob/main/inf-janet.el)

#### ajrepl

Supports at least:

* Various evaluation functions
* Recognition of Janet constructs including mutable things (e.g. `@{:a 1}`)
* Menu

In addition, there are some experimental features which can be enabled.

#### ijanet-mode

Supports various `ijanet-eval-*` functions.

#### inf-janet

There are at least two `inf-janet`s.  An older one which looks to be have
been based on `inf-lisp.el` and a more recent one that was based on
`inf-clojure.el`.

Note that they both require janet-mode.

##### inf-lisp.el based

Supports various `inf-janet-eval-*` functions.

##### inf-clojure.el based

Has support for at least:

* Various evaluation functions
* "Loading" a file (uses `import`)
* Displaying docstrings
* Completion
* Multiple janet process support
* Menu

### netrepl-based REPL

There are at least three implementations of netrepl-based REPL
connections:

* [a-janet-spork-client](https://github.com/sogaiu/a-janet-spork-client)
* [janet-netrepl](https://github.com/yrns/janet-netrepl)
* [snr](https://github.com/sogaiu/snr)

#### a-janet-spork-client

Supports netrepl connectivity and evaluation via Emacs Lisp.

#### janet-netrepl

Basic netrepl connectivity and evaluation via Emacs Lisp.

Note: have not verified this works in-depth.

#### snr

A simplified version of a-janet-spork-client that uses a proxy to
avoid implementing the netrepl protocol in Emacs Lisp.

## Linting

There is at least one Emacs Lisp package for linting Janet code:
[flycheck-janet](https://github.com/sogaiu/flycheck-janet)

### flycheck-janet

Integration of janet's built-in linter (`janet -k`) with Emacs via flycheck.

