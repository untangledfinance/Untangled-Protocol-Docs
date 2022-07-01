# Key terms

**Originator:** typically lenders who specialize in certain types of lending such as SME loans or trade finance. Other classes of Originators include Borrowers such as a developer of a renewable energy project.&#x20;

**Asset Pool**: a smart contract instance that purchases assets with its reserve in stable coins. Asset Pool borrows from Liquidity Pool (automatically) and Pool Backers (manually) (collectively called Funders) in order to purchase Assets from Originator. The interest of Funders within an Asset Pool could be represented by a Trustee, an independent and trusted third party in the real world.

**Borrower:** an entity that borrows from Asset Pool and uses the proceeds to develop a project, e.g. sustainability-linked loans where disbursement is made on-chain and a reward is available for achieving certain sustainability targets.

**Assets:** each Asset purchased by Asset Pool is represented by an NFT:

* An yield asset (such as a green project loan) is represented by LAT \

* A non-yield asset (such as a trade finance invoice) is represented by AIT\


**Validator:** a trusted entity that provides validation services re Assets: e.g. performing due diligence on assets being locked into an Asset Pool or certifying ‘collaterals’ such as loans, invoices or carbon credits.&#x20;

**Asset Pool Tranches**

* Senior tranche financing is represented by SOT, an ERC-20 token with a currency value of 1 but is continuously compounded with interest. \

* Junior tranche financing is represented by JOT, an ERC-20 token acting as the first loss piece in an Asset Pool. \


**Minimum First Loss**: a Asset Pool’s parameter that reflects minimum currency amount of JOT over Pool Value

**Reserve**: the value of stablecoins in a Asset Pool

**Pool Value**: equals Reserve plus Net Asset Value (&#x20;

**Backer**: Junior tranche investors (JOT token holders) who usually include Originator of a Asset Pool and other investors&#x20;

**Liquidity Pool:** a smart contract that receives stablecoins from Liquidity Providers and automatically lends to an Asset Pool once its minimum first loss has been reached i.e. the Borrowing has enough Backers, in exchange for Asset Pool’s SOTs. A Liquidity Pool can lend to many Asset Pools.&#x20;

**Funders:** Pool token holders (Liquidity Pool and Backers)

**Liquidity Provider**: Anyone supplying stablecoins to Liquidity Pool to receive passive fixed income represented by Liquidity Pool Token (LPU)

**Liquidity Pool Token (LPU):** an ERC20 token representing a unit share of assets of Liquidity Pool.&#x20;

**Liquidity Pool Bond:** LPB, an ERC20 token, is generated when a Liquidity Provider timelocks LPU into one of the available fixed expiration dates e.g. June 2022 i.e there will be LPB\_June 2022, LPB\_Sept 2022 and so on.&#x20;

**UTL:** Governance token of Untangled Protocol.
