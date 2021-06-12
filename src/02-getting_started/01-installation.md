## Installation
To use AbleScript, you need to download and compile it first. AbleCorp do not provide any binaries, so you have to clone the repository and build it.

### Install Rust Toolchain
First of all, if you didn't do it previously, you have to install Rust toolchain. That can be done using [Rustup](https://rustup.rs).

### Build AbleScript
First of all we need to get AbleScript sources and then build it:
```console
$ git clone https://github.com/AbleCorp/able-script
$ cd able-script
$ cargo build --release
```
The binary will be located in `target/release/` directory. You can also use `cargo run --release` to build and run it directly.