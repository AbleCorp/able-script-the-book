## Installation
To use AbleScript, you can download binary from AbleScript's repository (only x86_64 Linux) or build it yourself.

### Arch User Repository
You can build and install AbleScript from AUR: <https://aur.archlinux.org/packages/ablescript>

```console
> paru -S ablescript
```

### Binaries
You can download pre-build binaries from [here](https://git.ablecorp.us/AbleScript/able-script/releases).

Binaries are built for target `x86_64-unknown-linux-musl`.

You can verify binary's integrity by downloading `sha256sums` file and running:
```console
> sha256sum --check sha256sums
```

or by just computing and then comparing it manually
```console
> sha256sum ablescript-0.5.2-x86_64-unknown-linux-musl
7de28be2a50ace314ad32539eb2558bf4d4cea3c0fa172932e53de4a45400504  ablescript-0.5.2-x86_64-unknown-linux-musl
```

### Build
#### Install Rust Toolchain
First of all, you have to have Rust toolchain. It can be installed using [Rustup](https://rustup.rs).

#### Build AbleScript
First of all we need to get AbleScript sources and build it:
```console
> git clone https://git.ablecorp.us/AbleScript/able-script.git
> cd able-script
> cargo build --release
```
The binary will be located in `target/release/` directory. You can also use `cargo run --release` to build and run it directly.

## Interactive
When is AbleScript run without arguments, you can interactively execute code:
```console
> able-script
Hi [AbleScript 0.5.0]
:: 
```

For exiting, type `exit`