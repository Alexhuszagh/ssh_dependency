# ssh_dependency

An example Rust project with a private dependency.

Note that this project won't compile, since it depends on a private dependency my account has. The dependency is quite simple: it's a crate with only `Cargo.toml` and `src/lib.rs`.

**Cargo.toml**

```toml
[package]
name = "private_lib"
version = "0.1.0"
authors = ["Alex Huszagh <ahuszagh@gmail.com>"]
edition = "2018"
```

**src/lib.rs**

```rust
pub fn square(x: u32) -> u32 {
    x * x
}
```
