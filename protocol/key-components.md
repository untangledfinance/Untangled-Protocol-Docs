# Key components

![](https://lh5.googleusercontent.com/p0R-JQ6do6SIc-WBIegk-BFzbB0jf0UBZhnfZhPSmy0B2I2A5yZpKIJJaUHBEI-WiunF6fcmVcdRZ2muPxeR6dP-c8ZTycgbOD7tfNvy89iereN6P0JU0iqi9lL9KZV1fjaxGMiv9XUKIlvkVQ)

## Asset Pool

A smart contract that holds NFT’s representing loans and or invoices. These are the assets that are purchased at discount by the protocol, by Originator’s accessing funds from the Asset Pool. This Asset Pool has assets continually maturing and being purchased. So this tops up or drawdowns from the Liquidity Pool.

Asset Pool can have 2 tranches: senior (represented by SOT) and junior (JOT). Originator needs to retain some/all of the junior tranche to align interests in continuing to service Assets. Governance will determine the pool parameters including Originator’s JOT participation.

## Liquidity Pool

The Liquidity Pool is a smart contract for holding Liquidity Providers’ stablecoins, which underpins the liquidity for the Asset Pool to access. This Liquidity Pool takes in Liquidity Providers’ funds and gives them a Liquidity Pool token, LPU, which gives the holder a pro rata share to funds in the pool.&#x20;

Payment waterfall is represented by time locking the LPU. If a Liquidity Provider has a standard LPU, he can lock in the protocol’s Gauge contract, which enables locker to gain a boost in pro rata share of the Liquidity Pool’s stablecoin assets, corresponding to the expiry date of the locked LPU (in the form of Liquidity Pool Bond token, LPB). The further the expiry date the bigger the boost. This longer term lock in also provides a higher share of governance inflation, which allows the locker to have greater say in governance of originators.

## Governance Token

Early participants in JOT (Backers) and LPB (time locker of LPU) will also gain ongoing inflationary governance token, UTL.&#x20;

The inflationary governance token holders gain pro rata share of the protocol fees and can vote to add new borrowing and liquidity pools, including their parameters.  This also needs to give governance token holders greater say in managing credit risk in the asset pools, by ensuring they can have a say on retention or first loss by originator depending on risk.

Note that currently there is no plan for issuing UTL.
