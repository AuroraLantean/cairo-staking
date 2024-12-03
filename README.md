# cairo-staking

## Installation / Setup
scarb init

## Build and Test
```
scarb build
snforge test
```
## Deploying Contracts
copy the name of your seirra.json file in target/dev/ folder: staking1_cairo_token.sierra.json

```
starkli declare target/dev/staking1_cairo_token.sierra.json --compiler-version=2.1.0

starkli declare target/dev/staking1_cairo_token.sierra.json --rpc http://0.0.0.0:5050 --account ~/.starkli-wallets/deployer/account0_account.json --keystore ~/.starkli-wallets/deployer/account0_keystore.json
```

... Copy the class hash

## Docs
Starkli Docs: https://book.starkli.rs/introduction

Cairo Book: https://book.cairo-lang.org/title-page.html

Starknet Foundry Docs: https://foundry-rs.github.io/starknet-foundry/starknet/deploy.html
