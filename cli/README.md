# rwh - Rusty Wormhole 

A Rust implementation of the classic `magic-wormhole` command line client.

This package provides a library and a command-line tool named wormhole-rs, which makes it possible to get arbitrary-sized files and directories (or short pieces of text) from one computer to another. The two endpoints are identified by using identical "wormhole codes": in general, the sending machine generates and displays the code, which must then be typed into the receiving machine.

## Installation

### GitHub Releases

We publish source code and binaries to GitHub releases. Visit the [releases page](https://github.com/magic-wormhole/magic-wormhole.rs/releases) for the latest release.

Or use [cargo binstall](https://github.com/cargo-bins/cargo-binstall):

```bash
cargo binstall rwh
```

### crates.io

You can use cargo to install the CLI from crates.io:

```bash
cargo install --locked rwh
```

## Usage

```text
rwh 0.9.0 - Safe filetransfer through magic-wormhole
Usage: rwh [OPTIONS] <COMMAND>
Commands:
  send       Send a file or a folder [alias: s]
  receive    Receive a file or a folder [alias: r]
  send-many  Send a file to many recipients
  forward    Forward ports from one machine to another

Options:
  -v, --verbose   Enable logging to stdout, for debugging purposes
      --no-color  Disable color output
  -h, --help      Print help
  -V, --version   Print version


Run a subcommand with `--help` to know how it's used.
```
