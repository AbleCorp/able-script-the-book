## Installation
To use AbleScript, you need to download and compile it first. AbleCorp do not provide any binaries, so you have to clone the repository and build it.

### Install Rust Toolchain
First of all, you have to have Rust toolchain. It can be installed using [Rustup](https://rustup.rs).

### Build AbleScript
First of all we need to get AbleScript sources and build it:
```console
$ git clone https://github.com/AbleCorp/able-script
$ cd able-script
$ cargo build --release
```
The binary will be located in `target/release/` directory. You can also use `cargo run --release` to build and run it directly.

### Interactive
When is AbleScript run without arguments, you can interactively execute code:
```console
$ able-script
Hi [AbleScript 0.1.0] - AST Printer & Interpreter
:: 
```

> Currently, AbleScript prints AST before code execution

For exiting, type `exit`