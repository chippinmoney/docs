# ChippIn Docs | Rapyd Client - Rapyd Disburse API

> Rapyd Disburse provides methods for transferring money from a Rapyd Wallet to a beneficiary outside the Rapyd system.

Chippin supports [Payouts method](https://docs.rapyd.net/build-with-rapyd/docs/payouts) to deliver funds outside the Rapyd System.

## How It Works
The use-case for ChippIn users is when they are transfering money from their personal [Rapyd Wallet](https://docs.rapyd.net/build-with-rapyd/reference/rapyd-wallet-overview) to an external system or bank account. This is how it happens:

1. Users send fund transfer request.
2. Chippin Rapyd SDK supports execution of [Sender Object](https://docs.rapyd.net/build-with-rapyd/reference/sender-object) from users' wallet and delivers funds to destination defined in [Benficiary Object](https://docs.rapyd.net/build-with-rapyd/reference/beneficiary-object). There exists a thorough source and destination verification process for authentic and secure transactions that is described in the Rapyd Docs.