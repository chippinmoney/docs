# ChippIn Docs | Rapyd Client - Rapyd Collect API

> The payment is the basic mechanism for collecting money from customers and depositing it in the client wallet or other wallets.

The [Rapyd Collect API](https://docs.rapyd.net/build-with-rapyd/reference/rapyd-collect-overview) provides robust endpoints for users across any geographic location to transfer funds to ChippIn System without jumping over any currency excahange hassle.

## How It Works
When the users transfer funds from their external bank accounts or online wallets, ChippIn Rapyd Client has been developed to support [Payment Fees Object](https://docs.rapyd.net/build-with-rapyd/reference/payment-object#payment-fees-object) to complete the transaction. This is the flow:
1. Users send fund transfer request.
2. Chippin sends fund transfer request and generates [Rapyd Checkout Page](https://docs.rapyd.net/build-with-rapyd/reference/checkout-page-object).
3. Users execute final fund transfer.
4. Chippin uses [Payment Fees Object](https://docs.rapyd.net/build-with-rapyd/reference/payment-object#payment-fees-object) to complete the transaction.