# Protocol Components

### Issuer

An entity that borrows from Noteholders in order to purchase Assets from or lend directly to Project Borrower. The interest of the Noteholders within a Pool is represented by a Trustee, an independent and trusted third party.

### Originator

typically lenders who specialize in certain types of lending such as SME loans or trade finance. Other classes of Asset Originators include Project Borrower such as a developer of a renewable energy project.

### Noteholders

JOT Noteholder: provides first-loss capital to finance a Pool. SOT Noteholder: provides senior capital to finance a Pool Borrower: the entity that borrows from Issuer and uses the proceeds to develop a longer term project - think of sustainability linked loans where disbursement is made on-chain and reward is available for achieving sustainability targets.

### Validator

a trusted entity that provides validation services in relation to pool assets: e.g. due diligence the assets being uploaded to an Asset Pool or certifying on ‘collaterals’ such as carbon credits or renewable energy certificates

### Pool

A smart contract that holds individual non-fungible tokens from which Issuer issues senior tranche tokens and junior tranche tokens. A Pool can also hold tokens of other Pools.

### Pool Tokens

Each Asset supplied to the Pool is represented by a Non-Fungible Token (NFT):

* A yield asset (such as a green project loan) is represented by LAT
* A non-yield asset (such as a trade finance invoice) is represented by AIT

### Pool tranches

* Senior tranche financing is represented by SOT, which is an ERC-20 token with a start value of 1.
* First-loss (Junior) tranche financing is represented by JOT which is an ERC-20 token.

