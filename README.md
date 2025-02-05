# Janet Editor and Tooling Info

Mostly a collection of editor and tooling info for use with the Janet
programming language

## Background

It's possible to interact with a running `janet` process using what's
traditionally referred to as a REPL connection.  However, since
`janet` start-up is on the quick side, it's often doable just to
repeatedly start a succession of fresh `janet` processes.

See [here](doc/dev-styles.md) for more details.

## One Big List

If you just want to see the information as a `.tsv` file,
[here](listing.tsv) you go :)

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

## Editor-Independent Tooling and Bits

Below are some editor-independent tooling and bits with Janet support:

* Diffing - [difftastic](https://github.com/Wilfred/difftastic)

* Formatting
  * [jandent](https://github.com/sogaiu/jandent)
  * [janet-format](https://github.com/janet-lang/spork/blob/e598ef4c154974b9f15a1d632727389df4dccbd0/bin/janet-format) (part of spork)

* netrepl - [janet-netrepl](https://github.com/janet-lang/spork/blob/e598ef4c154974b9f15a1d632727389df4dccbd0/bin/janet-netrepl) (part of spork)

* Linting
  * `janet -k` aka [`flycheck` in `boot.janet`](https://github.com/janet-lang/janet/blob/dc325188d064f22e4a128b892eaf919289936eac/src/boot/boot.janet#L3953-L3967)
  * [review-janet](https://github.com/sogaiu/review-janet)

* LSP - [CFiggers' janet-lsp](https://github.com/CFiggers/janet-lsp)

* PEG
  * [janet-pegdoc](https://github.com/sogaiu/janet-pegdoc)
  * [margaret](https://github.com/sogaiu/margaret)
  * [small-peg-tracer](https://github.com/sogaiu/small-peg-tracer)

* Reference
  * [janet-ref](https://github.com/sogaiu/janet-ref)
  * [jdoc](https://github.com/sogaiu/jdoc)

* Syntax Highlighting
  * [pygments](https://github.com/pygments/pygments)
  * [rouge](https://github.com/rouge-ruby/rouge)

* tree-sitter - [tree-sitter-janet-simple](https://github.com/sogaiu/tree-sitter-janet-simple)

## Testing

Some testing options include:

* Simple assertion-based using `assert` and friends

  * janet does
    [this](https://github.com/janet-lang/janet/tree/f95de25b15e62cd54ad2bb676281a1321a823411/test)

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

  * [janet-ex-as-tests](https://github.com/sogaiu/janet-ex-as-tests) - simple example invocations that work as tests

## Benchmarking, Timing, Profiling

* [arnie](https://github.com/pyrmont/arnie) - run benchmarks on janet binaries
* [janet-benchmarksgame](https://github.com/MikeBeller/janet-benchmarksgame) - versions of the "computer language benchmarks game" benchmarks for janet
* spork's [timeit and timeit-loop](https://github.com/janet-lang/spork/blob/70f1a47281218ea21cfb81292e36a79b0c44e59c/spork/test.janet#L61-L103) - form execution timing
* [janet-profiling](https://github.com/saikyun/janet-profiling) - profiling of janet forms

## Credits

See [here](doc/credits.md) for helpful folks :)
