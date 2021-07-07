# ChippIn - Rapyd Client - Rapyd Wallet API

> The Rapyd Wallet (formerly known as eWallet) is a white-label digital wallet. Use it to receive, store, and send money. Brand the Rapyd Wallets with your own branding. Each wallet holds one or more accounts, each with its own currency and balance.

The [Rapyd Wallet API](https://docs.rapyd.net/build-with-rapyd/reference/rapyd-wallet-overview) is built for seamless transactions without any external verification screens and keep the users in the ChippIn system always.

The project makes use of **Buissness Type Wallet** to facilitate easy creation of Group Wallets and Personal Wallets.

## How It Works
When a wallet is created, the primary owner of the wallet is always ChippIn Admin. This way users can skip buisness-identity verification process and the process becomes seamless. Moreover, there is no additional advantage of being an admin to the users and eliminates any heirarchy within group members.

When the users transfer funds from their external bank accounts or online wallets, ChippIn Rapyd Client has been developed to support [Payment Fees Object](https://docs.rapyd.net/build-with-rapyd/reference/payment-object#payment-fees-object) to complete the transaction. This is the flow:
1. Users send fund transfer request.
2. If users are transfering funds to a group or anywhere within the Chippin System, [Wallet Transaction Object](https://docs.rapyd.net/build-with-rapyd/reference-link/wallet-transaction-object) is used to make the payment one-tap away.
3. If the users are transferring funds to their bank accounts, [Disburse API](Rapyd/disburse.md) is used.
4. If the users are transferring funds into the Chippin System, [Collect API](Rapyd/collect.md) is used.