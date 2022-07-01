# MakerDao MIP6 on trade finance assets

{% hint style="info" %}
**Good to know:** depending on the product you're building, it can be useful to explicitly document use cases. Got a product that can be used by a bunch of people in different ways? Maybe consider splitting it out!
{% endhint %}

#### Untangled Finance DROP: Diversified Trade Finance Fund

This MIP6 Proposal will finance a special purpose vehicle (“SPV”) established by [Untangled Finance 26](https://untangled.finance/) or affiliates thereof (the “Issuer”) to acquire Trade Finance (TFA) Assets.&#x20;

#### Summary <a href="#summary-2" id="summary-2"></a>

* UP Series LLC is a Digital Credit Fund set up by Untangled Finance, a digital securitisation platform. We partnered with Centrifuge as our technical infrastructure provider.
* The Series will be set up to invest in Trade Finance Assets (TFA). TFA are short term, self-liquidating invoice-based financing in both domestic and cross border trade. TFA traditionally has a [very low default rate 7](https://iccwbo.org/publication/icc-trade-register-report/#1550486691378-3a223d05-6e5e).
* TFA Series will invest in TFA from multiple asset originators. 3 originators have signed up to supply assets to the Fund. They have good underwriting records with zero default rate to date. All asset originators are subject to due diligence by Untangled and all due diligence material will be disclosed with the Maker RWF CU.
* UP Series LLC has developed a rigorous risk management framework:
  * Asset originator’s participation in Junior token is determined by institutional-grade reserve methodology developed by rating agencies.
  * Credit insurance will be applied where possible. The credit insurers will take the first loss in case of default.
* Substantial benefits for investors:
  * Maker
    * An ‘abstraction layer’ - Maker Governance won’t need to deal with individual asset originator’s applications → improve turnaround time
    * Scale up real-world adoption of Dai with proven, institutionally recognised structure and methodologies
  * Senior Investors (including Maker)
    * Diversification - avoid over concentration in a single originator, geography, borrower segment and collateral type
    * Safety - institutional-grade risk management framework consisting of 3 layers: credit insurer, junior participation and (in the case of Maker) over collateralisation of the DROP senior tranche in exchange for Dai
    * Transparency: daily on-chain portfolio performance tracking
    * Premium returns over equivalent investments

#### 1.Who is the interested party for this collateral application? <a href="#1who-is-the-interested-party-for-this-collateral-application-3" id="1who-is-the-interested-party-for-this-collateral-application-3"></a>

The Issuer, UP Series LLC, set up by [Untangled Finance 26](https://untangled.finance/), is represented by Quan Le ([untangled 26](https://untangled.finance/), or quan.le@untangled.finance, CEO at [Untangled Finance 26](https://untangled.finance/)) and Manrui Tang (manrui.tang@untangled.finance, COO at [Untangled Finance 26](https://untangled.finance/)). The issuer will source and manage TFA assets. It will create and own non-fungible tokens (“NFTs”) representing each TFA asset in the pool. It will lock their NFT’s into the Tinlake protocol to serve as collateral. The issuer will pool its assets and offer ERC-20 tokens to investors, specifically DROP Tokens & TIN Tokens.



1. Provide a brief high-level overview of the project, with a focus on the applying collateral token

[Untangled Finance 26](https://untangled.finance/), the Issuer/Asset Manager will originate new trade finance assets and use the Centrifuge’s [model 12](https://forum.makerdao.com/t/poll-rwa-working-group-centrifuge-model/4381) to use MCD as a liquidity provider to.

2.1 Collateral/Assets

* Trade finance assets secured by accepted invoices, inventory or revenues
* Asset term: Self-liquidating in 30 to 180 days
* Legal form: Accepted invoices, Promissory notes, Supply chain loans
* Security: Credit Insured where possible
* Default history: less than 0.5%

Trade finance gives investors access to a USD 15 trillion marketplace. This market has until recently been dominated by commercial banks. New regulations, however, have reduced their ability to meet demand. This has opened a window of opportunity to non-banking investors who want to enter a stable, well-established market that shows limited correlation to traditional credit classes.

With a financing gap of USD 3.4 trillion (USD 1.5 trillion pre COVID), the opportunities are abundant. In the current low-interest rate environment, there is growing demand for trade finance loans amongst institutional investors. This is also due to its efficient return on capital and [low 2](https://iccwbo.org/publication/icc-trade-register-report/#1550569973752-8879717c-dbf5) default history. When accessed in a robust and diversified way, and where care is taken to limit possible idiosyncratic or volatile risk factors such as commodity price risk, we believe it can be a powerful diversifier as part of a traditional credit allocation.

As an investment, trade finance loans exhibit a number of attractive characteristics. They offer a yield pick-up over other liquid credits and are very efficient from a solvency capital perspective. With most of such loans being self-liquidating (when invoice receivers pay, revenue collected through secured cash collection account), short-dated, and often secured, the asset class also offers protection against default risk and market risk should the cycle turn. Trade finance can also provide an effective platform to realize responsible investment objectives.

Asset selection: Only assets that fit certain criteria e.g. amount, duration, borrower type, credit rating etc will be selected to the pool. This is to further ensure no over concentration of borrower exposures, making the pool more diversified.

2.2 Pool Structure:

Untangled Finance has structured the pool to initially reflect a 90% vs 10% allocation to Senior & Junior, respectively. We structured the pool to ensure that there is sufficient coverage from Junior for the Senior tranche based on the characteristics of the underlying asset pool e.g. historical loss, average asset size, initial pool size for each asset originator selected to the pool.

[960×540 49.4 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/2/22b4b197b185f3daab0616ac2b494bb135e6a4c2.png)

![](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/2/22b4b197b185f3daab0616ac2b494bb135e6a4c2\_2\_624x351.png)

(1) Asset originator/lending partner makes an advance to a borrower.

(2)The asset originator accumulates a pool of assets then sells it to UP Series LLC.

(3) UP Series LLC issues Senior to investors according to the proposed parameters\*.

(4) The proceeds from investment will then be used to pay the asset originator.

(5) At the end of the asset term, the obligor/borrower repays the asset plus interest into a bank account of a SPV that is separate from the originator’s bank account.

(6) The SPV converts the money in its bank account to Dai to pay investors back principal plus interest.

2.3 Junior portion

Asset originators will participate in the higher risk part (called Junior, the ‘junior tranche’ or 3(b) in the diagram above). Because of this risk sharing by asset originators, there’s lower risk to investors if a borrower defaults. If this does happen, investors will be repaid (plus interest) before the asset originator’s share (Step (7) in the diagrams above).

2.4 Pool pricing

The pricing of the pool (DROP fixed APR) is determined by the yield of a debt instrument with an equivalent credit rating plus a premium.

2.5 Pool monitoring

Asset originators are subject to rigorous due diligence before on-boarding (a copy of DD reports will be shared with Centrifuge and the RWF CU of Maker). Once onboarded, asset originators need to fulfil daily reporting requirements via an API connection with the Untangled Platform (UP). It is possible to relevant legal clauses to automatic notification triggers on reporting covenants such as ratios of past dues, advance rate,

#### 3. Provide a brief history of the project <a href="#3-provide-a-brief-history-of-the-project-5" id="3-provide-a-brief-history-of-the-project-5"></a>

3.1 Untangled Finance

[Untangled Finance 26](https://untangled.finance/), through UP Series LLC, is a digital credit fund focusing on bridging real-world assets to DeFi and doing so at scale.

Our objective is to source a diversified asset portfolio that offers, at scale, strong returns, low risk and broaden access to asset classes that are traditionally reserved to institutional investors

We are specifically focusing on the following asset classes:

* Supply chain trade finance (this application)
* Green asset securitisation and green bonds issuance.
* SME Financing

Each asset class will be covered in a separate application.

TFA opportunities differ widely in terms of complexity, and investors need to understand the true risk drivers behind the attractive returns. Untangled has spent a considerable amount of time assessing the market and possible entry points. We are confident that the strategy we offer benefits from the attractive aspects of the asset class, whilst limiting much of the downside.

Trade finance differs from traditional corporate loan funds because they focus on specific sales, whereas normal corporate credit tends to be non-specific in terms of the use of funds. The financing of a specific sales contract rather than lending to a corporate is really the key to why [trade finance consistently outperforms credit 2](https://library.iccwbo.org/content/tfb/pdf/2019-icctraderegisterreport.pdf).

Our strategy differs from other trade finance funds in the market both in its underlying philosophy and in its investment process. Portfolio construction is aimed at properly diversifying risk whilst still allowing for a robust analysis of each transaction on responsible investing and compliance due diligence criteria.

We aim for a highly diversified portfolio in terms of geography, industry, and counterparties, which we regard as defensive in times of geopolitical uncertainty. We use an integrated approach to rating and risk analysis that builds off Untangled Finance’s significant expertise in credit, supplemented by advanced credit analytic models.

We set out the vision of tokenizing supply chain trade finance in this [whitepaper 8](https://drive.google.com/file/d/16NHTYt9ogGYZB6Nvv\_\_\_nykUgiaYxvao/view)

Key features of the Untangled Platform (UP)

[1600×927 146 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/168b97707db61708b167ee829e9290291a9cbac2.jpeg)

![](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/1/168b97707db61708b167ee829e9290291a9cbac2\_2\_536x310.jpeg)

UP is a one-stop shop for alternative lenders looking to raise funds and for investors to access alternative investment opportunities traditionally reserved for institutional investors. UP bridges real-world assets and DeFi.

Untangled Platform is to integrate directly with Centrifuge’s smart contracts providing seamless user experience.

* Originator On-boarding on Asset Tokenization

Once approved by a trusted third party, assets are tokenized as NFT/ ERC 721 tokens.

Asset-level data templates are in accordance with [European Central Bank](https://www.ecb.europa.eu/paym/coll/loanlevel/transmission/html/index.en.html). Consistent taxonomy and data representation enable meaningful comparisons for investors.

* Structuring Digital Asset

Using UP to structure a conforming digital asset by assessing asset eligibility criteria to maximise funding and optimise costs of funds. Users can run scenarios to optimise funding parameters and link the parameters to legal documentation.

* Investor On-boarding and Subscription

Investors are on-boarded to UP once they pass AML/KYC procedures appropriate for their jurisdictions.

Legal agreements are drafted based on standard templates and executed digitally on the platform.

* On-going performance tracking and investor reporting

Asset performance data such as repayment and an obligor’s finance position is dynamically updated to our platform via APIs. Issuers can set performance triggers based on smart legal clauses.

Investors have access to a real-time reporting dashboard where they can track asset-level data and on-going performance updates.

The Untangled Team:

Untangled has used established market relationships and tapped top industry advisors to build the Untangled Team:

Quan Le, Co-founder & CEO

More than 20 years in technology development, commodity trading and yield farming (for rice in Africa), financial engineering. Co-founded Binkabi, blockchain-based commodity trading and financing platform in 2017 and Untangled, digital securitisation platform. Masters Degree of Applied Finance and Investment; ACA qualification

Manrui Tang, Co-founder and COO

10+ year experience in blockchain, energy transition (to green), financial due diligence and M\&A advisory. Co-founded both Binkabi and Untangled with Quan. Previously with PwC and National Grid (UK). Degrees from London School of Economics and Imperial College; ACA qualification.

Tim Davies (Capital Markets, Structuring, and Securitisation Advisory. Investor)

Over 25 years experience in securitisation with global financial institutions including RBC Capital Markets, RBS, Lloyds, and NatWest Markets). Tim is recognised as a leading trade receivables funding expert, applying receivables financing techniques in the FinTech space over the past seven years to a variety of firms as a consultant and while at Demica, Demica Finance, NWM, and Blackstar Capital. Undergraduate Degrees from University of Toronto and an MBA(Hon) from York University (Canada).

3.2 Originator selection

[Untangled Finance 26](https://untangled.finance/) has partnered with a number of lending partners to originate the TFA assets globally. The following are in the initial batch of originators. The names of these and future originators will be revealed at a later date.

U\_Originator 1

Operating since 2016 in the Middle East, the company has helped small businesses that have limited/no access to bank finance with working capital lines in the form of invoice finance and vendor finance products. Within the e-commerce sector, the company has rolled out working capital solutions for marketplace sellers on Amazon (using the Fulfilled By Amazon model) and restaurants on food delivery apps such as Zomato, Talabat, Deliveroo. Based on revenue data on these platforms, the company makes short term, revolving credits, secured by future payments directly to the company’s bank account. To date, the company has funded over $15 million with zero loss.

U\_Originator 2

Here is an early payment company whose product allows suppliers to be paid early and buyers to extend their payment terms. Started in 2018 in Denmark the company is expanding to the Netherlands this year. The company was founded by an experienced team of business leaders, legal experts and software developers. The company’s credit exposures are 100% insured by Allianz ([AA rated by S\&P 1](https://www.allianz.com/en/investor\_relations/bonds/rating.html)). To date, the company has funded less than $10 million with zero loss.

U\_Originator 3

Launched in 2016 by its experienced board (100% owners) who have financed the technology sector (hardware) for 20 years with relationships at owner or board level into the industry’s leading international distributors and vendors; The company achieved 150% YOY growth. It offers trade finance facilities of USD1-15m to long established, stable distribution companies with strong trading histories operating in the growth markets of the Middle East, Southern and Eastern Europe and Asia. To date, the company has funded over $100 million with zero loss.



#### 4. Link the whitepaper, documentation portals, and source code for the system(s) that interact with the proposed collateral, and all relevant Ethereum addresses. If the system is complex, schematic(s) are especially appreciated. <a href="#4-link-the-whitepaper-documentation-portals-and-source-code-for-the-systems-that-interact-with-the-p" id="4-link-the-whitepaper-documentation-portals-and-source-code-for-the-systems-that-interact-with-the-p"></a>



#### 5. Link any available audits of the project. Both procedural and smart contract focused audits. <a href="#5-link-any-available-audits-of-the-project-both-procedural-and-smart-contract-focused-audits-7" id="5-link-any-available-audits-of-the-project-both-procedural-and-smart-contract-focused-audits-7"></a>



#### 6. Link to any active communities relating to your project. <a href="#6-link-to-any-active-communities-relating-to-your-project-8" id="6-link-to-any-active-communities-relating-to-your-project-8"></a>

* [Untangled Linkedin 1](https://www.linkedin.com/company/untangled-finance/?viewAsMember=true)

#### 7. How is the applying collateral type currently used? <a href="#7-how-is-the-applying-collateral-type-currently-used-9" id="7-how-is-the-applying-collateral-type-currently-used-9"></a>

The SPV will be financed by issuing DROP Tokens for 90% of the net asset value of the pool of NFTs plus cash on hand (collectively “Pool Valuation”) and TIN Tokens for 10% of the Pool Valuation.

The Issuer will initially seek a 10 million DAI debt ceiling from MakerDAO, increasing to a 20 million DAI over the next 6-12 months. We expect to fill up this initial 10 million dai within 6 months based on our existing pipeline with our lending partners.

The Issuer expects to invest in TFA assets that are typically less than 6 months. Upon the self liquidation of TFA assets, the Issuer will repay the outstanding balance drawn against the NFT and accrued interest thereon.

#### 8. Does one organization bear legal responsibility for the collateral? What jurisdiction does that organization reside in? <a href="#8-does-one-organization-bear-legal-responsibility-for-the-collateral-what-jurisdiction-does-that-org" id="8-does-one-organization-bear-legal-responsibility-for-the-collateral-what-jurisdiction-does-that-org"></a>

Legal Setup

Untangled Finance will form its own SPV (UP Series LLC) for the acquisition of TFA assets. The SPV will enter into a service agreement with Untangled Finance Limited to get support from Untangled Finance while using Centrifuge’s open and decentralized infrastructure. The SPV will tokenize the titles of each of its TFA Assets into NFTs and will add those NFTs to Tinlake as collateral. The SPV will utilize Tinlake to issue U-DROP and U-TIN backed by the pool of NFTs that are locked in Tinlake. Untangled Finance’s lending partners will retain the U-TIN tokens and will lock the U-DROP tokens into a MakerDAO Vault. Please find the documentation to the two-tranche structure [here 3](https://developer.centrifuge.io/tinlake/overview/tranches/).

This legal setup is very commonly used in the traditional financial system: The collateral for the individual assets are assigned to a legal entity, the “special purpose vehicle” and lenders get an ownership interest in the entire portfolio of this entity (with this entity the assets are in an a bankruptcy-remote structure that is not influenced by the Asset Originators) and provides the necessary support to ensure that anyone that owns a DROP token has a legal claim to the underlying assets.

#### 9. Where does exchange for the asset occur? <a href="#9-where-does-exchange-for-the-asset-occur-11" id="9-where-does-exchange-for-the-asset-occur-11"></a>

The SPV enters into a subscription agreement with lenders who receive DROP from the SPV in turn for providing DAI. The DROP token can be redeemed against the cash flows of the underlying collateral directly from the SPV by any DROP holder. This is ensured by the Tinlake smart contracts and is the primary way for interacting with these tokens.

1. (Determined by Legal Domain Team) Has your project obtained any legal opinions or memoranda regarding the regulatory standing of the token or an explanation of the same from the perspective of any jurisdiction? If so, those materials should be provided for community review.

First, the issuance of DROP and TIN tokens is handled via Tinlake, with AML/KYC procedures and compliance with US securities guidelines. Investors based in the US must be accredited investors (generally defined as having a net worth of at least $1 million).

The offering structure overview and legal templates can be found [here 1 5](https://docs.centrifuge.io/tinlake/further-information/offering-structure/).

#### 11. (Determined by Legal Domain Team) Describe whether there are any regulatory registrations for the token and provide related documentation (including an explanation of any past or existing interactions with any regulatory authorities, regardless of jurisdiction), if applicable. <a href="#11-determined-by-legal-domain-team-describe-whether-there-are-any-regulatory-registrations-for-the-t" id="11-determined-by-legal-domain-team-describe-whether-there-are-any-regulatory-registrations-for-the-t"></a>

The issuance of DROP and TIN tokens is handled via Tinlake, with AML/KYC procedures and compliance with US securities guidelines. Investors based in the US must be accredited investors (generally defined as having a net worth of at least $1 million). The SPV issues DROP tokens for the Maker vault.

#### 12. (Optional) List any possible oracle data sources for the proposed Collateral type. <a href="#12-optional-list-any-possible-oracle-data-sources-for-the-proposed-collateral-type-13" id="12-optional-list-any-possible-oracle-data-sources-for-the-proposed-collateral-type-13"></a>

The Issuer will provide daily NAV updates for each underlying TFA asset, which will be used to value the NFTs.

If an updated NAV submitted by the Issuer shows a decrease in the total expected value of an underlying TFA asset, then the value of the NFT will be marked down. If, as a result of such mark down, the outstanding value of the DROP Tokens increases to more than 90% of the Pool Valuation, then Tinlake will lock the Issuer from drawing any further Dai and will lock the TIN investors from redeeming. The Issuer may restore balance and unlock Tinlake by: (1) buying additional TIN tokens so that the proceeds will increase the cash reserve in an amount necessary to cause the value of outstanding DROP Tokens to be no more than 90% of the Pool Valuation or (ii) redeem DROP Tokens in an amount necessary to restore the value of outstanding DROP Tokens to no more than 90% of the Pool Valuation.

#### 13. (Optional) List any parties interested in taking part in liquidations for the proposed Collateral type. <a href="#13-optional-list-any-parties-interested-in-taking-part-in-liquidations-for-the-proposed-collateral-t" id="13-optional-list-any-parties-interested-in-taking-part-in-liquidations-for-the-proposed-collateral-t"></a>

Bankruptcy protection: even if the originator goes out of business, the loans are still safe as borrowers make repayment directly to the SPV’s bank account. We propose a Maker participate of up to 75% of DROPwith the remainder being provided by direct DROP investors

[960×540 40.3 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/5/5f3a21dc1a9cb24febe7b9990a02a4c2c8757579.png)

![](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/5/5f3a21dc1a9cb24febe7b9990a02a4c2c8757579\_2\_624x351.png)

From an overall pool perspective, Maker gets four buffers of safety:

* Credit insurance on most assets with payout at 90% first loss
* 10% TIN tranches held by Asset Originators, Untangled and Centrifuge
* DROP co-investors, who share Maker interests
* DROP over-collateralisation i.e., 105 U-DROP for 100 DAI

Note: Opportunities only available to accredited and professional investors.
