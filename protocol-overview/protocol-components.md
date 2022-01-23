# Protocol Components

{% hint style="info" %}
**Good to know:** your product docs aren't just a reference of all your features! use them to encourage folks to perform certain actions and discover the value in your product.
{% endhint %}



### Issuer&#x20;

An entity that borrows from Noteholders in order to purchase Assets from or lend directly to Project Borrower. The interest of the Noteholders within a Pool is represented by a Trustee, an independent and trusted third party.&#x20;

### Originator&#x20;

typically lenders who specialize in certain types of lending such as SME loans or trade finance. Other classes of Asset Originators include Project Borrower such as a developer of a renewable energy project.

### Noteholders&#x20;

JOT Noteholder: provides first-loss capital to finance a Pool. SOT Noteholder: provides senior capital to finance a Pool Borrower: the entity that borrows from Issuer and uses the proceeds to develop a longer term project - think of sustainability linked loans where disbursement is made on-chain and reward is available for achieving sustainability targets.&#x20;

### Validator&#x20;

a trusted entity that provides validation services in relation to pool assets: e.g. due diligence the assets being uploaded to an Asset Pool or certifying on ‘collaterals’ such as carbon credits or renewable energy certificates&#x20;

### Pool&#x20;

A smart contract that holds individual non-fungible tokens from which Issuer issues senior tranche tokens and junior tranche tokens. A Pool can also hold tokens of other Pools.&#x20;

### Pool Tokens&#x20;

Each Asset supplied to the Pool is represented by a token:&#x20;

* A yield asset (such as a green project loan) is represented by LAT
* A non-yield asset (such as a trade finance invoice) is represented by AIT

### Pool tranches&#x20;

* Senior tranche financing is represented by SOT, which is an ERC-20 token with a start value of 1.
* First-loss (Junior) tranche financing is represented by JOT which is an ERC-20 token.&#x20;

Whale Protocol represents a modular solution for a complete value chain in bridging crypto liquidity pools to real world assets. The modules are:&#x20;

Liquidity Pool&#x20;

A system of smart contracts responsible for managing full cycle of issuing note tokens, calculating token price based on net asset value to redeeming token for investors&#x20;

Asset Origination: smart contracts that manage the full cycle of tokenising debts (loan asset token), calculating interests accrued to managing the repayment through either Agent Origination Model (Originator sells assets to Pool) or Direct Origination Model (Pool lends directly to end Borrower)&#x20;

PUMP governance token that aligns interests among key participants, bootstraps the network and acts as a risk backstop. In the following sections we will discuss each of these modules in turn.
