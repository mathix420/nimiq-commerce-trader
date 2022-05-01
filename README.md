# nimiq-commerce-trader
Automatically send Nimiq to kucoin to be swapped for stablecoin.


# WIP

## Steps

1. User buy something on your store via a Nimiq transaction.
2. A serverless script then check if the transaction is validated.
3. If validated, the whole Nimiq amount is then send to kucoin to be traded.
4. A script will then perform a trade with the choosen pair. For example NIM/BUSD.
5. That's it, your transaction is now safe from volatility!

## Specs

- Platform agnostic
    - Terraform ?
    - Serverless Framework ?
- Better if serverless
- Need to be customizable
    - Choose pairs 

## Ideas

- It might be simpler to directly use the Kucoin Nimiq address as recipient for the first transaction. Then check if the transaction is made and valid, and perform a kucoin trade.
    - If the address subject to changes, then use the kucoin API to get the address before each store transactions.
