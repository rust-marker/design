[back](./README.md)

# How will lints be provided/discovered

## To start

- Lints will be included as a dependency using Cargo.toml and available from crates.io.
- The lint crates are compiled as dylibs and dynamically linked to the lint driver.
- Naming works like any other crate; it needs to be unique (think `lint-regex` not `regex`); existing rules bind us.


## Future

- Possibility of pre-compiled registry
- Integration into cargo/crates.io or the registry may give more flexibility with naming and auto-detection

### Example in Cargo.toml
```toml
[package.metadata.lints]
auto-detect = false # true would eliminate the need for `foo` and `bar` below if they are already dependencies

[package.metadata.lints.crates]
foo = "0.2.0"
bar = "0.16.0"
_internal = { path = "..." }
```
