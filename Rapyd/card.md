# ChippIn Docs | Rapyd Client - Rapyd Card API

> The Rapyd Issuing platform provides the following interfaces between standard banking services and Rapyd Wallets.

Chippin supports [Issued Card Object](https://docs.rapyd.net/build-with-rapyd/reference/issued-card-object) to issue cards from external bank card.

## How It Works
The use-case for ChippIn users would be able to use their Chippin Funds and make any transactions outside Chippin System using Rapyd Provided Cards. This is how it happens:

1. Users send card issue request.
2. Chippin Rapyd SDK supports execution of [Issued Card Object](https://docs.rapyd.net/build-with-rapyd/reference/issued-card-object) from users' wallet and delivers funds to card.
3. Rapyd API is used to [activate issued cards](https://docs.rapyd.net/build-with-rapyd/reference/issued-card-object#activate-issued-card).
4. [PIN Code is set for card](https://docs.rapyd.net/build-with-rapyd/reference/issued-card-object#set-pin-code) and it is ready to use.
