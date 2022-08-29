# Namesdao .xch Wallet, a fork of chia-blockchain

Namesdao .xch Wallet is a fork of the Chia reference wallet, which adds support for Namesdao .xch names and outgoing memo's for XCH transactions.

Namesdao wallet is from Namesdao, a DAO which is not affiliated with the company Chia Network.


Python 3.7+ is required. Make sure your default python version is >=3.7
by typing `python3`.



##Install from source

*This instruction is for MacOS, Ubuntu, CentOS, RedHat, WSL2, Amazon Linux 2 and possibly *NIX like OSes.

```# Prerequisite: git

git clone https://github.com/theNamesdao/namesdao-wallet.git --recurse-submodules
cd namesdao-wallet

# This installs compatible Python modules
sh install.sh
. ./activate

# This installs supported version NodeJS/npm and npm dependencies.
sh install-gui.sh

# To open GUI app, run the following command
bash start-gui.sh
```

If you are behind a NAT, it can be difficult for peers outside your subnet to
reach you when they start up. You can enable
[UPnP](https://www.homenethowto.com/ports-and-nat/upnp-automatic-port-forward/)
on your router or add a NAT (for IPv4 but not IPv6) and firewall rules to allow
TCP port 8444 access to your peer.
These methods tend to be router make/model specific.

Most users should only install harvesters, farmers, plotter, full nodes, and wallets.
Setting up a seeder is best left to more advanced users.
Building Timelords and VDFs is for sophisticated users, in most environments.
Chia Network and additional volunteers are running sufficient Timelords
for consensus.


## Chia blockchain

Chia is a modern cryptocurrency built from scratch, designed to be efficient, decentralized, and secure. Here are some of the features and benefits:
* [Proof of space and time](https://docs.google.com/document/d/1tmRIb7lgi4QfKkNaxuKOBHRmwbVlGL4f7EsBDr_5xZE/edit) based consensus which allows anyone to farm with commodity hardware
* Very easy to use full node and farmer GUI and cli (thousands of nodes active on mainnet)
* [Chia seeder](https://github.com/Chia-Network/chia-blockchain/wiki/Chia-Seeder-User-Guide), which maintains a list of reliable nodes within the Chia network via a built-in DNS server.
* Simplified UTXO based transaction model, with small on-chain state
* Lisp-style Turing-complete functional [programming language](https://chialisp.com/) for money related use cases
* BLS keys and aggregate signatures (only one signature per block)
* [Pooling protocol](https://github.com/Chia-Network/chia-blockchain/wiki/Pooling-User-Guide) that allows farmers to have control of making blocks
* Support for light clients with fast, objective syncing
* A growing community of farmers and developers around the world

Please check out the [wiki](https://github.com/Chia-Network/chia-blockchain/wiki)
and [FAQ](https://github.com/Chia-Network/chia-blockchain/wiki/FAQ) for
information on this project.
