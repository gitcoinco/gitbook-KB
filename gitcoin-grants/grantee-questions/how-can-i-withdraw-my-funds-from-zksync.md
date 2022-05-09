---
description: >-
  Withdrawing funds from zkSync differs depending on the type of wallet you
  have.
---

# 🏧 How can I withdraw my funds from zkSync?

### Withdraw funds from a regular account

If your address is a regular externally owned account; you should visit [zkSync's Wallet page](https://wallet.zksync.io) and withdraw them in the browser.

### Withdraw funds from a smart contract account

If your contract can execute arbitrary transactions, you can email Matter Labs ([hello@matter-labs.io](mailto:hello@matter-labs.io)) or hop in [the zkSync Discord](https://discord.com/invite/px2aR7w) to ask about the best way to connect it to zkSync (assuming you can't connect it from [https://wallet.zksync.io/](https://wallet.zksync.io/\)))

Alternatively, if you just want to withdraw funds to L1, you can use [the zkSync force exit npm package](https://www.npmjs.com/package/zksync-force-exit-cli). This will let any account force push funds from zkSync to L1 if the address has never interacted with zkSync.

You can do this with:

```
npm install -g zksync-force-exit-cli
zksync-force-exit -k <privateKeyOfAddressToSendTxFrom> -a 
<addressToWithdrawZkSyncFundsFrom> -t <tokenSymbol> -n mainnet
```
