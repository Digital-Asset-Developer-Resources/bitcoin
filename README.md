Blockchain Resources - Bitcoin
==============================

https://bitcoin.org


What is Bitcoin?
-----------------
Bitcoin is an innovative payment network and a new kind of money.  [Documentation](https://bitcoin.org/) and [Github](https://github.com/bitcoin/bitcoin).


Network Configurations
----------------------

There are four major types of networks available with various [configuration options](https://jlopp.github.io/bitcoin-core-config-generator/).

1. [Full archival Mainnet](configuration/archival_node.json) with all transactions indexed (txindex=1) and blocks - 8CPU/32Gb/300Gb
2. Default [pruned Mainnet](configuration/default.json) with last 1000 blocks and all account balances -  2CPU/4Gb/5Gb
3. [Testnet](configuration/testnet.json) with [faucet](https://tpfaucet.appspot.com/)
4. [Regtest](https://bitcoin.org/en/glossary/regression-test-mode) A local testing environment in which developers can almost instantly generate blocks on demand for testing events, and can create private satoshis with no real-world value.

Search in AWS region ***us-east-2*** for public AMIs with name ***SRP
Bitcoin***.  Copy/paste the ami-id into the image loader; e.g. [python
AMI](https://github.com/Digital-Asset-Developer-Resources/aws/blob/master/python/AMI.ipynb).
Alternatively, follow these [instructions](nodes/README.md) for the
AWS UI.

Mainnet nodes take about 6 hours to sync using a 8CPU/32GB
(t2.x2large) EC2 instance on AWS.  Catch up after 2 days takes about 6
minutes, not including txindex reindexing.

* On December 28, 2019; Bitcoin sync from genesis to block 61202 took
  from 14:31:27 - 20:13:36, or an elapsed time of 05:42:09 with full
  archival Mainnet configuration.
  

Capabilities
------------

Capabilities include wallet support, including multi-sig wallets,
transfers with finality on the order of 1 hour as well as platform
tokens; e.g. the [omni layer](https://www.omnilayer.org/); [atomic
swaps](https://lightning.network/), JSON/RPC interface and SDKs.

### Tokens

The token standard, [omni layer](https://www.omnilayer.org/) is an open-source, fully-decentralized asset platform on the Bitcoin Blockchain.

### Atomic Swaps

Scalable, Instant Bitcoin/Blockchain Transactions using the [Lightning Network](https://lightning.network/)


### CLI


### SDK


