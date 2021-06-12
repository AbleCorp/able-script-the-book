## Installation
To use AbleScript, you need to download and compile it first. AbleCorp do not provide any binaries, so you have to clone the repository and build it.

### Install Rust Toolchain
First of all, if you didn't do it previously, you have to install Rust toolchain. That can be done using [Rustup](https://rustup.rs).

### Download and compile AbleScript
To get AbleScript sources, you have to clone it from its GitHub repo.
```console
$ git clone https://github.com/AbleCorp/able-script
```
Optionally, you can switch to different branch with newer features (and possibly more bugs), for example
```console
$ git checkout interpreter-fixes
```

Then, after you cloned the repository, use Cargo to build it. Use `--release` flag, to build optimised, production binary.
```console
$ cargo build --release
```
The binary will be located in `target/release/able-script`. You can also use `cargo run --release` to build and run it directly.