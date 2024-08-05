# 💡 Transfer Project Ownership

You may eventually need to transfer ownership of a project to a different address. This can be done interacting with the Allo smart contracts directly.

**Note:** In order to execute the following transaction, you must be the owner of the project- typically the account that created t.

To transfer project ownership, follow these steps:

1.  Visit Registry contract address `0x4AAcca72145e1dF2aeC137E1f3C5E3D75DB8b5f3` on a block explorer for your desired chain.

    Example: [Arbitrum](https://arbiscan.io/address/0x4AAcca72145e1dF2aeC137E1f3C5E3D75DB8b5f3#writeProxyContract)\


    <figure><img src="../../.gitbook/assets/Screenshot 2024-08-01 174208.png" alt=""><figcaption></figcaption></figure>
2. Visit the **Contract** tab, then **Write as Proxy**, and **Connect to Web3** (pictured above).\

3. Open the **updateProfilePendingOwner** method, and enter your parameters:
   * `profileId` can be found in the Builder URL for your project→ https://builder.gitcoin.co/#/chains/\<chainID>/registry/0x/projects/**`profileID`**
   * `pendingOwner` should be a wallet address you control, and will be the new owner after the process is complete.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

4.  Click **Write** and execute the transaction.

    Warning: if you receive a similar message below, there is likely an error in the transaction. Double check the parameters, and that your connected wallet is the Program creator.

    <figure><img src="../../.gitbook/assets/image (21).png" alt="" width="230"><figcaption></figcaption></figure>
5. **From the new wallet**, visit the same Registry contract address from Step 1 and ensure the Connected Web3 Wallet is for the new address.
6. Open the **acceptProfileOwnership** method, and enter your parameter:
   * `profileId` should be the same as Step 3

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

7. Click **Write** and execute the transaction.

Your new address should now be able to see and control the project from within [Builder](https://builder.gitcoin.co/).
