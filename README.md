# Ethereum Notes

Quick Ethereum Reference

## Blockchain

Blockchain

## Wallets

Seed, private keys, public keys, addresses

## Transactions

Every transaction on Ethereum requires computational resources to execute, so each transaction requires a fee in order to be included in a block.

Transaction Fee = Gas Price * Gas Used by transaction

The gas price is the cost in Ether (expressed in Gwei) of one unit of gas that you are ending up paying for the transaction to be included in a block.

The gas used by transaction refers to the unit that measures the amount of computational effort required to execute specific operations on the Ethereum network. It must be lower to the gas limit, which is the maximum amount of gas units you are willing to pay for in order to carry out a transaction or EVM operation.

Gas Price = Gas Base Fee + Gas Max Priority Fee

The gas base fee which is the minimum gas price a transaction must pay to be a valid transaction (it changes per block, depending on how full the previous block is). The Base Fee is burned so the block producer (miner/validator) does not receive any of it. It is algorithmically adjusted to try to target for all the blocks to be 50% full.

Ethers Burnt = Gas Base Fee * Gas Used by transaction

The gas max priority fee goes to the validator when the transaction is included in a block, and incentivizes them to prioritize your transaction. It is a maximum amount because the block producer may be paid less. One way this can happen is by specifying a gas max fee, which is the total fee a transaction is willing to pay.

Tip to Miners = Gas Max Priority Fee * Gas Used by transaction

The gas max fee is the absolute maximum you are willing to pay per unit of gas to get your transaction included in a block. The gas price you are ending up paying is a little bit lower than the Gas Max Fee.

## Consensus Mechanism

PoS
