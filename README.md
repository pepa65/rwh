[![version](https://img.shields.io/crates/v/rwh.svg)](https://crates.io/crates/rwh)
[![build](https://github.com/pepa65/rwh/actions/workflows/push.yml/badge.svg)](https://github.com/pepa65/eqr/actions/workflows/push.yml)
[![dependencies](https://deps.rs/repo/github/pepa65/rwh/status.svg)](https://deps.rs/repo/github/pepa65/rwh)
[![docs](https://img.shields.io/badge/docs-rwh-blue.svg)](https://docs.rs/crate/rwh/latest)
[![license](https://img.shields.io/badge/License-EUPLv1.2-blue.svg)](https://github.com/pepa65/eqr/blob/main/LICENSE)
[![downloads](https://img.shields.io/crates/d/rwh.svg)](https://crates.io/crates/rwh)

# rwh 0.9.0
**Rusty Wormhole - Safe filetransfer through magic-wormhole**

* See <http://magic-wormhole.io/>
* Rust port of the Python version: <https://github.com/magic-wormhole/magic-wormhole>
* After: <https://github.com/magic-wormhole/magic-wormhole.rs>
* Repo: <https://github.com/pepa65/rwh>
* License: EUPL v1.2 or later




## Miscellaneous Information
### Comparison with the Python implementation
Features that are missing:
* Text message sending
* Folder sending (we can send folders, but it will send a tar ball which the other side will have to manually unpack)
* Tor support

New features that exceed the other implementations:
* Can do direct connections across the internet (NATs) and firewalls
* Automatically copies your code to the clipboard
* Port forwarding in addition to file transfer (experimental)
* Send a file to multiple people (experimental)
* Fuzzy wormhole code completion

### Developing
If you want to toy with the CLI, `cargo run -- --help` will get you started. The code sits in `./cli/src`. For more instructions see [cli/README.md](cli/README.md).

If you'd like to use Wormhole in your application, `cargo doc --open` will tell you how to use it. There aren't any hosted docs at the moment.

If you don't fear touching code and want to contribute, `./src/lib.rs`, `./src/transfer.rs` and `./src/transit.rs` are rather easy to get into. The [protocol specification](https://github.com/magic-wormhole/magic-wormhole-protocols) will probably be useful to you.

### Applications using Wormhole Rust as library
* [Warp](https://gitlab.gnome.org/World/warp), a GUI client using Gtk
* [Wormhole File Transfer](https://github.com/wormhole-app/wormhole), a Android client using Flutter
* [Wyrmhole](https://github.com/ClaytonWas/wyrmhole), a cross-platform GUI using Tauri
* [rvIRC](https://github.com/KaraZajac/rvIRC), a vim-based IRC client with filesharing
* Feel free to add yours!

### License
This work is licensed under the EUPL v1.2 or later. Contact the owner(s) for use in proprietary software.

