# Create Pool

Anyone can create a pool which is a smart contract instance where an Issuer can:&#x20;

* Borrow from Noteholders.
* Purchase assets from Originators (Agency origination model) with Pool Reserve or lend to Borrowers (Direct Origination Model)&#x20;

Pool creator needs to specify parameters such as:&#x20;

* Pool currency: currency that both Asset tokens (LAT, AIT) and financing tranches (SOT, JOT) are denominated in. Currently the Protocol support DAI and USDC stable coins
* &#x20;Minimum first loss ratio: expressed as a percentage of Pool Value, this is the minimum currency amount of Junior Tranche.&#x20;
* Originator: Approved address(es) who can supply Assets to the Pool.
