# Janet Editor and Tooling Info

## One Big List

If you just want to see the information as a `.tsv` file,
[here](listing.tsv) you go :)

## Development Styles

It's possible to interact with a running janet process using what's
traditionally referred to as a REPL connection.  However, since
`janet` start-up is on the quick side, it's often doable just to
repeatedly start a succession of fresh `janet` processes.

See [here](doc/dev-styles.md) for more details.

## Editors and Such

There is support for Janet (to varying degrees) for:

* [CudaText](doc/cudatext.md)
* [Emacs](doc/emacs.md)
* [Helix](doc/helix.md)
* [Kakoune](doc/kakoune.md)
* [Neovim](doc/neovim.md)
* [Sublime Text](doc/sublime-text.md)
* [TIC-80](doc/tic-80.md)
* [Vim](doc/vim.md)
* [VSCode](doc/vscode.md)

## Editor-Independent Tooling

Below are some editor-independent tools with Janet support that I've
seen some use of:

* Diffing - [difftastic](https://github.com/Wilfred/difftastic)

* Formatting
  * [jandent](https://github.com/sogaiu/jandent)
  * [janet-format](https://github.com/janet-lang/spork/blob/e598ef4c154974b9f15a1d632727389df4dccbd0/bin/janet-format) (part of spork)

* netrepl - [janet-netrepl](https://github.com/janet-lang/spork/blob/e598ef4c154974b9f15a1d632727389df4dccbd0/bin/janet-netrepl) (part of spork)

* Linting
  * `janet -k` aka [`flycheck` in `boot.janet`](https://github.com/janet-lang/janet/blob/dc325188d064f22e4a128b892eaf919289936eac/src/boot/boot.janet#L3953-L3967)
  * [review-janet](https://github.com/sogaiu/review-janet)

* Misc Reference Helpers
  * [janet-pegdoc](https://github.com/sogaiu/janet-pegdoc)
  * [janet-ref](https://github.com/sogaiu/janet-ref)
  * [jdoc](https://github.com/sogaiu/jdoc)

* LSP - [CFiggers' janet-lsp](https://github.com/CFiggers/janet-lsp)

* Syntax Highlighting
  * [pygments](https://github.com/pygments/pygments)
  * [rouge](https://github.com/rouge-ruby/rouge)

* tree-sitter - [tree-sitter-janet-simple](https://github.com/sogaiu/tree-sitter-janet-simple)

## Testing

Some testing options include:

* Simple assertion-based using `assert` and friends

  * [janet does
    this](https://github.com/janet-lang/janet/tree/f95de25b15e62cd54ad2bb676281a1321a823411/test)

  * [spork/test](https://github.com/janet-lang/spork/blob/c1953f6d01cedfaea78a0c54b7748e33823a8592/spork/test.janet)
    (evolved from above?)

* Somewhat similar functionality using `deftest` and friends

  * [testament](https://github.com/pyrmont/testament) - "takes
    inspiration from Joy's Tester library and Clojure's clojure.test
    library"

* Other

  * [judge](https://github.com/ianthehenry/judge) - "library for
    writing inline snapshot tests"

  * [golden-master](https://github.com/yumaikas/golden-master) -
    "[golden-master](https://en.wikipedia.org/wiki/Characterization_test)
    testing library for Janet."

  * [janet-usages-as-tests](https://github.com/sogaiu/janet-usages-as-tests) - simple usage examples that work as tests

## Credits

See [here](doc/credits.md) for helpful folks :)
