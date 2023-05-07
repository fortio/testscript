# Testscript
Script-based testing based on txtar files (now/here a toplevel module)

 * Provides a shell-like test environment that is very nicely tuned for testing Go CLI commands.
 * Extracted version of the core Go team's internal testscript package.
 * Heavily used to test the `go` command.
 * Includes patterns for checking stderr/stdout, command pass/fail assertions, and so on.
 * Built-in support for Go concepts like build tags.
 * Integrates well with `go test`, including coverage support.
 * Inputs and sample outputs are in the [txtar](https://pkg.go.dev/golang.org/x/tools/txtar) text archive format, also used by the Go playground.
 * Accompanied by a testcript command for running standalone scripts with files embedded in txtar format.

A great introduction to using testscripts is this [blog post](https://bitfieldconsulting.com/golang/test-scripts) series.

Also included are the following:

- imports: list of known architectures and OSs, and support for reading import statements.
- par: do work in parallel.
- testenv: information on the current testing environment.
- testscript: 

This is a fork/hacked up version of https://github.com/rogpeppe/go-internal as a toplevel testscript/ minimal module - keeping up with upstream with a few minor changes (like allowing "!foo" to work instead of requiring "! foo" etc)

## Links
<!-- 
note this shows up in Links header section of https://pkg.go.dev/fortio.org/testscript 
so while redundant with the above inline link, let's keep that section (TIL)
-->

- [Test scripts in Go](https://bitfieldconsulting.com/golang/test-scripts)
