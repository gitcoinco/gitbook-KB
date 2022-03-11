# How can I withdraw my funds from zksync?

If your address is a simple account; head over to [http://wallet.zksync.io/](http://wallet.zksync.io/) and withdraw them in browser!

If not, it's a smart contract... read on:

If your contract can execute arbitrary transactions, you can email Matter Labs \(hello@matter-labs.io\) or hop in their Discord [https://discord.gg/px2aR7w ](https://discord.gg/px2aR7w) to ask about the best way to connect it to zkSync \(assuming you can't connect it from [https://wallet.zksync.io/](https://wallet.zksync.io/%29)\)

Alternatively, if you just want to withdraw funds to L1, easiest way is like to use their npm package. This will let any account force push funds from zkSync to L1, if the address has never interacted with zkSync. 

You can do this with:

```text
npm install -g zksync-force-exit-cli
zksync-force-exit -k <privateKeyOfAddressToSendTxFrom> -a 
<addressToWithdrawZkSyncFundsFrom> -t <tokenSymbol> -n mainnet
```

