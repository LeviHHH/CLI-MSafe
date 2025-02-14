# CLI-MSafe

The CLI interface for interacting Momentum Safe. This repository majorly has two components:

1. The CLI interface for users to interact with Momentum Safe. 
2. The underlying typescript SDK of for smart contract interaction.

## Installation

Clone the repository and change directory:

```
git clone git@github.com:Momentum-Safe/CLI-MSafe.git
cd CLI-MSafe
```

Install dependencies:

```
yarn install
```

## Quick start

### Install Aptos CLI tools. 

The CLI tool is used for setting up the initial account. Install with github release or compile from source. 

* [Github release](https://github.com/aptos-labs/aptos-core/releases?q=cli&expanded=true) (Recommended)
* [Install from source](https://aptos.dev/cli-tools/aptos-cli-tool/install-aptos-cli)

### Initialize a wallet

Use aptos CLI to setup the wallet and environment. 

```
aptos init 
```

Choose all default settings to create a new wallet with the devnet endpoint settings.

The command will create a config file `.aptos/config.yaml` under the current directory, which includes 
the wallet information as well as the network endpoint message.

### Start Momentum Safe CLI 

```
yarn start
```

And follow the instructions to operate with momemtum safe.

## Interact with Momentum Safe

The following features are currently supported by Momentum Safe:

1. Momentum Safe creation
2. APT coin transfer
3. View momentum safe owned by the account
4. View pending transactions of the momentum safe
5. Coin registry.
6. Coin transfer of any coin type.
7. Custom MOVE module interaction (For simple types).
8. MOVE module publish.
9. Revert transaction.
10. Asset list.

We will add more features shortly:

1. Add coin decimal and bigint
2. Add more custom ABI, struct, e.t.c.



