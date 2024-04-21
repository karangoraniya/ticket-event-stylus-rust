# EventPass Platform on Stylus Arbitrum Sepolia (Work in Progress)

This is the README for the EventPass Platform, currently under development for ticketed events. While the ERC20 token functionality is completed, other features are still in progress.

## Introduction

The EventPass Platform is designed to facilitate the organization and management of events that require ticketing. Built on the DEvent Ticket platform, it leverages the capabilities of ERC20 tokens for ticket issuance and management.

## Stylus Testnet on Arbitrum Sepolia

The EventPass Platform is compatible with the Stylus testnet on the Arbitrum Sepolia network. This testnet environment provides a sandbox for developers to test and deploy their contracts before going live. By utilizing Arbitrum Sepolia, developers can ensure the security and functionality of their contracts in a controlled environment.

## Deployment

### Cloning the Repository

To get started, clone the repository from GitHub:

```bash
git clone https://github.com/karangoraniya/ticket-event-stylus-rust
```

### Exporting ABI

You can export the Solidity ABI for the contract using the `cargo stylus` tool:

```bash
cargo stylus export-abi
```

### Checking Compilation and Deployment Readiness

Before deploying the contract, ensure it compiles to valid WASM for Stylus and will succeed in deployment on-chain. Use the following command to check:

```bash
cargo stylus check
```

### Deploying to Stylus Testnet

Deploy the contract to the Stylus testnet using the `cargo stylus deploy` command. Make sure to specify your private key path and use the `--estimate-gas-only` flag for gas estimation:

```bash
cargo stylus deploy \
  --private-key-path=privatekey.txt \
  --estimate-gas-only
```

Note: Don't forget to add your private key file to the .gitignore file to prevent it from being committed to the repository.

Make sure to replace `privatekey.txt` with the path to your private key file.

## ERC20 Ticket Management

The contract incorporates ERC20 functionalities for ticket management. This allows for the creation, transfer, and redemption of tickets using standard ERC20 methods.

For further details on contract usage and functionalities, refer to the documentation or explore the codebase.

```

This README provides a concise overview of the EventPass Platform on Stylus Arbitrum Sepolia, its deployment process on the Stylus testnet using Arbitrum Sepolia, and its integration with ERC20 for ticket management.
```
