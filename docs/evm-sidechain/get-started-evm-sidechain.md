---
html: get-started-evm-sidechain.html
parent: evm-sidechains.html
blurb: Get started with the EVM compatible sidechain for the XRP Ledger.
labels:
  - Development, Interoperability
status: not_enabled
---
# Get Started with the EVM Sidechain

<embed src="/snippets/_evm-sidechain-disclaimer.md" />

This getting started tutorial walks you through the steps to set up your account and submit a transaction using the EVM sidechain bridge. 

## 1. Create an Account Using an EVM Compatible Wallet
<!-- STYLE_OVERRIDE: wallet -->

In order to interact with the network, you need to create an account in the EVM sidechain. To create and manage this account you can use any EVM compatible wallet such as MetaMask.

For instructions on how to install and create an account using MetaMask, see [Connect MetaMask to XRP Ledger EVM Sidechain](connect-metamask-to-xrpl-evm-sidechain.md).


## 2. Assign your XRP Ledger Devnet Tokens to the EVM Sidechain

Before you can start interacting with the EVM blockchain, you need to assign some of your XRP Ledger Devnet Tokens to the EVM Sidechain. 

To generate tokens in the XRP Ledger Devnet, go to the [XRP Faucets](https://xrpl.org/xrp-testnet-faucet.html) page and click **Generate Devnet credentials** to generate a new Devnet account with some test XRP in it.

![Generate XRP Ledger Devnet credentials](../img/evm-sidechain-xrpl-devnet-faucet.png '#width=300px;')

Note the address and secret associated with your Devnet address. You need this information to set up your preferred XRP Ledger wallet. 


## 3. Submit a Transaction Using the EVM Sidechain Bridge

Once you have your accounts set up and test fund allocated, submit a transaction to assign some of your test tokens from the XRP Ledger Devnet to the EVM Sidechain using the EVM Sidechain bridge.

The EVM Sidechain bridge is a tool that enables transactions between chains in a fast and secure way.


### 1. Connect Both Wallets


**Connect Xumm Wallet**

Use your Xumm wallet to interact with the XRP Ledger Devnet chain.
Ensure that you have created an account on the public XRP Ledger Devnet as described in Step 1. 

To connect a Xumm wallet to the bridge, go to [EVM sidechain bridge](https://beta.bridge.devnet.xrpl.org) and click **Connect Xumm Wallet**.

![Connect XUMM Wallet](../img/evm-sidechain-connect-xumm-wallet.png '#width=500px;')


**Note:** Ensure that you are connected to XRP Ledger Devnet and that the application that you are connecting with is the correct one.

Follow the instructions on screen to scan the QR code using the Xumm app. The Xumm wallet app displays a confirmation page.

![Connect to XRP Ledger Devnet](../img/evm-sidechain-bridge-sign-in.jpg '#width=300px;')


**Connect MetaMask Wallet**

Use your MetaMask wallet to interact with the XRP Ledger EVM Sidechain. 
Ensure that you have created a MetaMask account and connected to the public XRP Ledger Devnet as described in [Connect MetaMask to XRP Ledger EVM Sidechain](connect-metamask-to-xrpl-evm-sidechain.md).

To connect a MetaMask wallet to the bridge, go to the [EVM sidechain bridge](https://beta.bridge.devnet.xrpl.org) and click **Connect Metamask Wallet**.

![Connect MetaMask Wallet](../img/evm-sidechain-connect-metamask.png '#width=300px;')


### 2. Start the Transaction 

Now that both Xumm and MetaMask wallets are connected to the bridge, you can select the direction of the bridge, the amount, and the address to fund.

- **Direction of the bridge**: The direction can be either EVM sidechain → XRP Ledger Devnet or XRP Ledger Devnet → EVM sidechain. Use the **Switch Network** button to switch the direction.
- **From Amount**: This is the transaction amount. Note that there is a fee to use the bridge.
    - Network fees: The fees required by the network for your transactions.
    - Commission: The bridge applies a commission for every transaction completed. This is to prevent spam and distributed denial of service attacks (DDOS).
- **Destination Address**: The address on the chain where you want the funds.

    ![Start the transaction](../img/evm-sidechain-initiate-transfer.png '#width=500px;')

Enter the details for your transaction and click **Transfer**. Review the details of the transaction carefully before accepting the transaction in the corresponding wallet. 

![Approve the transaction](../img/evm-sidechain-approve-transaction.png '#width=500px;')

Once you approve the transaction in either the Xumm Wallet or Metamask (depending on the direction of the transfer), a loading screen displays. This process can take up to a few minutes.

![Transaction in progress](../img/evm-sidechain-transfer-in-progress.png '#width=500px;')


### 3. Receive the Funds

After a few minutes of transaction processing time, you are redirected to the **Transaction Confirmation** screen where you can verify the details of the bridge transaction.

- **Origin transaction hash**: Hash of the transaction in the origin chain.
- **Destination transaction hash**: Hash of the transaction in the destination chain.
- **From address**: Address on the origin chain.
- **To address**: Address on the destination chain.
- **Receive**: The amount received in the destination address.

![Transaction confirmation](../img/evm-sidechain-transaction-confirmation.png '#width=500px;')

Your transaction has completed successfully and the test XRP tokens are now available in the other chain.
