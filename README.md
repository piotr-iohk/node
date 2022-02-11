# node + wallet set up on TESTNET

1. You need to have `cardano-node` and `cardano-wallet` on your `$PATH`. You can get binaries for your OS from [Cardano-wallet release page](https://github.com/input-output-hk/cardano-wallet/releases). Cardano-wallet release archive includes both `cardano-wallet` and `cardano-node` (also few other handy tools, like `cardano-cli`, `cardano-addresses` or `bech32`).


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
