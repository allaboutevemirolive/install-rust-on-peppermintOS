# Install-rust-on-peppermintOS


This repository is dedicated to myself as I'm often migrate between operating system from one to another.

First thing first, we have to resolve a few issues:

## 1. Uninstall the system-wide installation of Rust: 

Uninstall any system-wide installation of Rust to avoid conflicts with Rustup . To do this, you can run the following command:

```
sudo apt-get remove rustc
```
This will remove the system-wide installation of Rust from your system.

## 2. Use Rustup to manage your Rust installation: 

Instead of relying on a system-wide installation of Rust, you can use `Rustup` to manage your Rust toolchains and install Rust components like `Rustfmt`. 

To do this, you can follow the installation instructions for Rustup at [https://rustup.rs](https://rustup.rs/).

The page will ask you to run the command somehting like below:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Once Rustup is installed, you can use it to install Rustfmt by running the following command:

```
rustup component add rustfmt
```
This will install Rustfmt as a Rust component that can be used with any Rust toolchain managed by Rustup.

## 3. Use a Rust version manager: 

Another option is to use a `Rust version manager` like multirust or rustup.shim to manage your Rust installations. 

These tools can coexist with a system-wide installation of Rust and allow you to switch between different Rust toolchains and installations as needed. 

You can find more information on using a Rust version manager in the [Rust documentation](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html#working-with-nightly-rust).



