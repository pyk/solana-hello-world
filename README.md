# Solana On-chain Program

My first Solana on-chain program.

## Resources

- [Solana - Developing with Rust](https://docs.solana.com/developing/on-chain-programs/developing-rust)
- [Solana - Hello Word App](https://github.com/solana-labs/example-helloworld)

## Build & Test

Use the following command to build the on-chain program:

    cargo build-bpf --manifest-path=./Cargo.toml --bpf-out-dir=program

To run the unit tests:

    cargo test

There are two kinds of unit tests: [Exercising program function directly](./src/lib.rs) and [testing in an environment that more closely matches a live cluster](./tests/lib.rs).

## Deploy

    solana program deploy /home/pyk/solana_hello_world/program/solana_hello_world.so
