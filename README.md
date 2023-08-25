## Foundry

![Github Actions][gha-badge]

[gha-badge]: https://img.shields.io/github/actions/workflow/status/Sunscreen-tech/foundry/check.yml?branch=sunscreen

Foundry consists of:

- [**Forge**](./crates/forge): Ethereum testing framework (like Truffle, Hardhat and DappTools).
- [**Cast**](./crates/cast): Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- [**Anvil**](./crates/anvil): Local Ethereum node, akin to Ganache, Hardhat Network.
- [**Chisel**](./crates/chisel): Fast, utilitarian, and verbose solidity REPL.

## Sunscreen

This repo contains Sunscreen's fork of Foundry. Everything is the same, except
that the underlying EVM supports additional [precompiles][precompile-repo] so
that you can perform FHE computation.

## Installation

Installing our fork is simple!
First, [get Rust](https://www.rust-lang.org/tools/install). Then

```sh
cargo install --git https://github.com/Sunscreen-tech/foundry --profile local forge anvil cast chisel
```

Or, if you've already cloned down this repo, you can install from local paths:

```sh
cargo install --path ./crates/forge --profile local --force --locked
cargo install --path ./crates/anvil --profile local --force --locked
cargo install --path ./crates/cast --profile local --force --locked
cargo install --path ./crates/chisel --profile local --force --locked
```

## Documentation

For documentation, refer to the [Foundry Book][foundry-book] and the original
[Foundry README][foundry-repo].

[precompile-repo]: https://github.com/Sunscreen-tech/fhe_precompiles
[foundry-book]: https://book.getfoundry.sh
[foundry-repo]: https://github.com/foundry-rs/foundry
[foundry-gha]: https://github.com/foundry-rs/foundry-toolchain
[ethers-solc]: https://github.com/gakonst/ethers-rs/tree/master/ethers-solc/
[solmate]: https://github.com/transmissions11/solmate/
[geb]: https://github.com/reflexer-labs/geb
[vaults]: https://github.com/rari-capital/vaults
[benchmark-post]: https://www.paradigm.xyz/2022/03/foundry-02#blazing-fast-compilation--testing
[convex]: https://github.com/mds1/convex-shutdown-simulation
[vscode-setup]: https://book.getfoundry.sh/config/vscode.html
[shell-setup]: https://book.getfoundry.sh/config/shell-autocompletion.html
