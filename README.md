# Wasmswap Interface Example Asset List

> :warning: **If you were previously using token_list you may need to migrate to pools_list to use the latest version of wasmswap**: To generate pools_list off of tokens_list and rewards_list (optionally) use the [assets merger](https://github.com/Wasmswap/assets-list-merger) 

These files are used by the Wasmswap interface to determine which assets are available and find relevant chain information. Direct links to these files should be configured in the Wasmswap env file.

## Important Security Info

Before adding any assets, query the contract and ensure it is instantiated from the proper byte code. The metadata should also be checked with `wasmd q wasm contract <contract-address>` to ensure an admin is not set as this could put users liquidity at risk. 

## Pools List

This file determines the assets & pools available.

## IBC Assets

This file determines the assets that can be deposited and withdrawn via IBC.

## Chain Info

This file provides configuation to Keplr for interacting with the chain.
