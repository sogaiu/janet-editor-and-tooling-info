# Development Styles

## REPL Connections

For using a REPL connection, there are primarily two options.  One is
communicating with a janet process using stdio and the other is via
netrepl.

The stdio option doesn't require anything special as it is built into
the janet executable.  Launching the janet binary with no arguments
should yield a typical REPL prompt.

The server side of the netrepl connection requires extra tooling.
Likely, this will be via the spork library which comes with the
`janet-netrepl` script which wraps spork's netrepl server
functionality.  Apart from the ability to connect over a network, a
notable benefit of the netrepl approach is better asynchronous
behavior compared to that of the stdio connection.

In both case there is the usual downside of potentially unexpected
behavior due to state mutation, but this option can still be useful.

## Multiple Fresh Janet Processes

The approach of repeatedly starting a new Janet process has the
advantage of always starting from a clean state.

As long as the start-up (or restoration of state) cost remains low
enough, the human waiting time between "restoration" can remain
tolerable.  This depends on the project in question, but often in the
early stages of development it may not be a significant issue.

There is also the possibility of employing [a rather different
approach to
development](https://ianthehenry.com/posts/my-kind-of-repl/).

## Stating the Obvious

Needless to say, there's not much stopping one from using either
approach depending on the situation :)
