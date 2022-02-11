# node + wallet set up on TESTNET

1. You need to have `cardano-node` and `cardano-wallet` on your `$PATH`. You can get binaries for your OS from release page of each project in GH.
 - [Cardano-node releases](https://github.com/input-output-hk/cardano-node/releases)
 - [Cardano-wallet releases](https://github.com/input-output-hk/cardano-wallet/releases)
> :information_source: Check out [compatibility matrix](https://github.com/input-output-hk/cardano-wallet#latest-releases) to make sure you have compatible versions of each.
>

2. Get configs:

```bash
git clone https://github.com/piotr-iohk/node.git
cd node/bin
./wget-config testnet
```

3. Start node:
```bash
cd node/relay1
./start_node 0.0.0.0 9999
```

4. Start wallet:
```bash
cd node/wallet
./wallet_start 8090 relay1
```
