# Ethereum The Merge

## What is The Merge
- POW to POS
- ETH1 -> execution layer
- Beacon chain -> consensus layer

## Why merge
- Power consumption - 99% less energey than POW
- Scalability - Prepare for sharding
- Decentralization - secured by 422k+ validators
  - 30% by Lido - 4.2M ETH
  - 15% by Coinbase - 2M ETH
  - 8% by Kraken - 1.1M ETH
  - 7% by Binance - 904,608 ETH
  - 40% by others

## How to merge (Mainnet)
- Clients
  - Execution layer
    - Geth (go)
    - Erigon (go)
    - Besu (java)
    - Nethermind (c#)
  - Consensus layer
    - Lighthouse
    - Teku
    - Prysm
    - Nimbus
- Bellatrix upgrade (consensus layer) - Activated on Sept 6
- Difficulty bomb
  - TTD (Total Terminal Difficulty):     ==58750000000000000000000==
  - [The Merge TTD](https://notes.ethereum.org/@MarioHavel/merge-ttd)
  - Difficulty @2022-09-08 03:12:16 UTC: ==58258959264202236971210==
  - Typical difficulty: 12496385052092057

## What will happen after The Merge?
- Gas fee
- TPS
- Mining machines
- Existing DApp
- Layer2
- MEV

## Roadmap
[Understanding The Merge, Surge, Verge, Purge, And Splurge](https://volt.capital/blog/the-merge)
- The Merge
- The Surge
  - Sharding
  - ZK Rollup
- The Verge - Verkle Tree
- The Purge - Expire historical data
- The Splurge - Proposal Builder Seperation

## ETH Fork
- ETHW
  - Supported by Chandler Guo宝二爷 and Justin Sun(孙割)
  - Disable TTD
  - Change EIP-1559
  - Freeze LP
  - Chain ID
    - Mainnet: 10001
    - Testnet: 10002 - 10005
- ETHW support
  - Miner
    - [Ethermine -End of Ethereum PoW Mining Phase](https://ethermine.org/announcement)
  - Layer2
    - Will not support
  - DApp
    - Almost all DApp will ==NOT== support ETHW
    - [AAVE Stops Loaning ETH Ahead of Merge](https://beincrypto.com/aave-stops-loaning-eth-ahead-of-merge/)
    - [Pause ETH Borrowing](https://app.aave.com/governance/proposal/97/)
  - CEX
    - MEXC
    - Gate.io
    - Poloniex
  - Other

- Pricing impact / trend

- Tech deep dive
  - Beacon chain
    - Consensus
      - PBFT
      - Gasper
        - Casper FFG ()
        - LMD-GHOST (Latest Message Driven - Greedy Heaviest-Observed Sub-Tree)
    - Commitee
      - at least 128 validators
      - 16 validators becomes aggregator
    - Attestation
      - 1.Generation
      - 2.Propagation
      - 3.Aggregation
      - 4.Propagation
      - 5.Inclustion
    - Slot
      - 12 seconds
      - 64 committees per slot
    - Epoch
      - 32 slots
      - 6.4 minutes
    - Fanality
      - need 2 epochs
    - RANDO
  
    - Incentive
      - Reward
        - Attestation
        - Block proposal
      - Slash
  
    - Block structure
      - consensus header
      - old block

  - Testnet
    - Goerli - Aug 10
    - Sepolia - July 6
    - Ropsten - June 8 - will be deprecated in Q4 2022

  - Verkle Tree
    - State storage
      - Merkle Tree
      - Merkle Partricia Tree
      - Verkle Tree
    - State expiration
    - Stateless clients
    - Data Avalability

## Todo
- research how to migrate validator (efforts, cost, tech feasability)