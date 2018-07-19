# Running a private Ethereum blockchain

This repo contains files and instructions for starting a private Ethereum blockchain network.

## Prerequisites / Dependencies

1) Install [Homebrew](https://brew.sh/)
2) Install [Geth](https://github.com/ethereum/go-ethereum/wiki/geth) using Homebrew, like this:
```bash
brew tap ethereum/ethereum
brew install ethereum
```

## Start an Ethereum Node
```bash
# Insantiate your data directory
geth --datadir ./myDataDir init ./myGenesis.json

# Start your node
geth --rpc --rpccorsdomain "http://localhost:8000" --datadir ./myDataDir --networkid 1994 console 2>> myEth.log
```
