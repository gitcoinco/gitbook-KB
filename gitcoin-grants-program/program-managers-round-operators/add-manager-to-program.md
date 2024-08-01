# 💡 Add Manager to Program

Program Managers have similar permissions to the Program Admin (creator). They can create rounds and edit program metadata, but _cannot_ add other Managers.

**Note:** In order to execute the following transaction, you must be the owner of the program - typically the account who created the program.

To add a member to your program, follow these steps:

1.  Visit Registry contract address `0x4AAcca72145e1dF2aeC137E1f3C5E3D75DB8b5f3` on a block explorer for your desired chain

    Example: [Arbitrum](https://arbiscan.io/address/0x4AAcca72145e1dF2aeC137E1f3C5E3D75DB8b5f3#writeProxyContract)\


    <figure><img src="../../.gitbook/assets/Screenshot 2024-08-01 174208.png" alt=""><figcaption></figcaption></figure>
2. Visit the **Contract** tab, then **Write as Proxy**, and **Connect to Web3** (pictured above).\

3. Open the **addMembers** method, and enter your parameters:
   * `profileId` can be found in the Manager URL for your program → https://manager.gitcoin.co/#/program/**`profileId`**
   * `members` should be a list of wallet addresses that you want to add as managers to your program, separated by commas. A single address can be entered as below.

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

4.  Click **Write** and execute the transaction.

    Warning: if you receive a similar message below, there is likely an error in the transaction. Double check the parameters, and that your connected wallet is the Program creator.

    <figure><img src="../../.gitbook/assets/image (21).png" alt="" width="230"><figcaption></figcaption></figure>

