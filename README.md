[![Rust](https://github.com/Trenrod/book_zerotoproduction/actions/workflows/rust.yml/badge.svg?branch=develop)](https://github.com/Trenrod/book_zerotoproduction/actions/workflows/rust.yml)

# Zero to Production

## Setup

### Code coverage 

Install with 
```
# At the time of writing tarpaulin only supports
# x86_64 CPU architectures running Linux.
cargo install cargo-tarpaulin
```

Execute
```
# With tests
cargo tarpaulin

# Without tests
cargo tarpaulin --ignore-tests
```

### Linting

Install/Enable
```
rustup component add clippy
```

Run
```
cargo clippy
```

In CI pipeline
```
cargo clippy -- -D warnings
```
