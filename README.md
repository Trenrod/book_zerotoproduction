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
