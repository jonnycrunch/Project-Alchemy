# Project Alchemy

An effort to bring together the [Zcash](https://z.cash/) and [Ethereum](https://ethereum.org) blockchains

## ZRelay

A [BTC Relay](http://btcrelay.org/)-inspired Zcash SPV client on the EVM

The Zcash PoW consists of two components which must be implemented in the EVM. [BLAKE2b](https://blake2.net/blake2.pdf), a cryptographic hash function, is used in the [Equihash](https://z.cash/blog/why-equihash.html) Proof-of-Work system.

There is a Solidity implementation of BLAKE2b and Equihash in this repo, and an [EIP](https://github.com/ethereum/EIPs/issues/129) for a BLAKE2b precompiled contract for efficiency.

### Tests:

Install Dapple (version >= 0.8)

    npm install -g dapple

Run tests

    dapple test


## zkSNARKS

Another priority is the incorporation of [zkSNARKs](https://github.com/scipr-lab/libsnark) directly into the EVM. An EIP for this is forthcoming, following the ideas and implementation work done in the [Baby ZoE](https://github.com/zcash/babyzoe) project.
