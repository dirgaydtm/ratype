# Contributing

Thanks for helping out.

## Setup

```sh
rustup target add wasm32-unknown-unknown
cargo run        # terminal
trunk serve      # web
```

On Linux the terminal build needs the ALSA development files (`libasound2-dev` or `alsa-lib`). See [ARCHITECTURE.md](ARCHITECTURE.md) for the code layout.

## Before a pull request

```sh
cargo fmt
cargo clippy -- -D warnings
cargo clippy --target wasm32-unknown-unknown -- -D warnings
cargo test
```

Keep the change small and follow the style of the code around it.
