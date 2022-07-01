# MakerDAO- Collateral Onboarding Risk Evaluation

{% hint style="info" %}
****

[teej](https://forum.makerdao.com/u/teej)[Real World Finance Core Unit](https://forum.makerdao.com/g/Real-World-Finance)[Dec '21](https://forum.makerdao.com/t/untangled-finance-collateral-onboarding-risk-evaluation/12006?u=quntangled)

RWA collateral onboarding risk evaluation template

_Legal Disclaimer: This communication is provided for information purposes only. This communication has been prepared based upon information, including market prices, data and other information, from sources believed to be reliable, but such information has not independently been verified and this communication makes no representations about the enduring accuracy of the information or its appropriateness for a given situation. This content is provided for informational purposes only, and should not be relied upon as legal, business, investment, financial or tax advice. You should consult your own advisers as to those matters. References to any digital assets and the use of finance-related terminology are for illustrative purposes only , and do not constitute any recommendation for any action or an offer to provide investment, financial or other advisory services. This content is not directed at nor intended for use by the MakerDAO community (“MakerDAO”), and may not under any circumstances be relied upon when making a decision to purchase any other digital asset referenced herein. The digital assets referenced herein currently face an uncertain regulatory landscape in not only the United States but also in many foreign jurisdictions, including but not limited to the UK, European Union, Singapore, Korea, Japan and China. The legal and regulatory risks inherent in referenced digital assets are not the subject of this content. For guidance regarding the possibility of said risks, one should consult with his or her own appropriate legal and/or regulatory counsel. Charts and graphs provided within are for informational purposes solely and should not be relied upon when making any decision. The content speaks only as of the date indicated. Any projections, estimates, forecasts, targets, prospects, and/or opinions expressed in these materials are subject to change without notice and may differ or be contrary to opinions expressed by others._

### Executive summary <a href="#executive-summary-1" id="executive-summary-1"></a>

**Debt Ceiling**: 20MM DAI\
**Stability Fee**: S+4.0%\*\
**Advance Rate**: 95%\
**Asset SPV Credit Enhancement**: 5%\
**Minimum Maker Vault On-Chain Credit Enhancement**: 5%\
**Term**: 2-year vault/credit line\
**Liquidation Process**: Contingent on legal structure\
**Maker Vault Maximum All-In LTV**: 85.74%

Check the [RWA Documentation 8 9](https://docs.google.com/document/d/1Khm\_K9S10Z7xobJimR9rx2MuUaW-txWy8FLzWfTLaG0/edit) for more information.

For Untangled’s MIP-6 and Collateral Onboarding Call, see the below links:

[MIP-6 8](https://forum.makerdao.com/t/mip6-application-untangled-finance-drop-u-drop-diversified-trade-finance-fund/9167)\
[Collateral Onboarding Call 9](https://forum.makerdao.com/t/collateral-onboarding-call-34-untangled-friday-july-30-4pm-utc/9527)

**Preface**

The below assessment represents a credit assessment, not an exhaustive feasibility study. Ultimately, the launch of a Maker Vault will require a subsequent A) legal review and B) a technical/smart contract review.

As per a recent[ poll 5](https://forum.makerdao.com/t/consultation-poll-centrifuge-global-debt-ceiling-cap/11619), the community has expressed discontent with deals that utilize “old” legal structures. Accordingly, the transition of a “yay” vote on this risk assessment to an active vault will be contingent upon the DAO’s approval of a new and acceptable legal structure. The specific parameters of what constitutes an “acceptable” structure have not yet been established.

In the case of this collateral application, a bespoke structure will be installed and paid for by the arranger (Untangled). The novel legal structure will most certainly affect the liquidation mechanism associated with the collateral that secures the Maker vault. Untangled has proposed a legal structure which will be submitted to the community for approval if and only if this risk assessment is approved.

Please focus your evaluation of the below report solely on the innate credit characteristics of the opportunity. To exercise judgement independent of the ambient uncertainty in the DAO is to demonstrate a commitment to the onboarding of high-quality, diverse assets.

### Highlights <a href="#highlights-2" id="highlights-2"></a>

UP Series LLC is a digital credit fund operated by Untangled Finance, a digital asset securitization platform regulated by the Financial Conduct Authority in the UK. If approved, Untangled will serve as an arranger who sits between MakerDAO and the originators of trade finance assets (TFAs), particularly those that enable the international trade of tangible goods and commodities. We can regard this structure as an early opportunity to utilize the [Arranger Model 4](https://forum.makerdao.com/t/the-arranger-model-a-highly-scalable-rwa-framework/11298).

Quan Le and Manrui Tang will head Untangled. The fund will participate, via deployment of credit lines/revolvers, in assets originated by underlying asset originators who provide liquidity solutions and trade credit to SMEs. The purpose of this short-term credit is to improve cash conversion cycles and solve working capital needs. Untangled will focus on the origination of self-liquidating, short-term (30-120 day) assets backed by invoices, inventory, or revenue. Prior to Untangled, the founders launched (2017) and operated Binkabi, an agricultural supply chain FinTech company.

This structure will implement a proprietary (to Untangled) technical solution that supports the tokenization of underlying trade finance assets. Untangled Finance has structured UP Series LLC as an SPV that will source trade finance cash flows from the underlying asset SPVs. Trade finance assets are tokenized at the asset SPV level (where promissory notes are issued) to support transparency, alignment, and the avoidance of cross-collateralization. As of now, the platform intends to onboard an initial cohort of four asset originators.

For resources/refreshers on trade finance, see the below links:

[Trade Finance Basics 3](https://www.youtube.com/watch?v=OHvOyUGcC5Y)\
[Commodity/Inventory Finance](https://www.youtube.com/watch?v=idh6F3KveFY)\
[How Blockchains Can Improve Trade Finance 4](https://www.youtube.com/watch?v=nhozN3YGMb4)

### What is the essence of this opportunity? <a href="#what-is-the-essence-of-this-opportunity-3" id="what-is-the-essence-of-this-opportunity-3"></a>

The risks intrinsic to the Untangled proposition should be weighed against its opportunities.

**Primary Risks:**

* **Execution Risk**: Untangled is functionally a start-up without a history of credit performance. While both principals have expertise applicable to the task at hand, neither comes strictly from a credit background. These realities cast doubt on the fund’s capacity to deploy prudent capital at scale and monitor outstanding exposure rigorously.
* **Industry Risk**: Because Untangled is focused on international trade finance, it necessarily inherits the complications that cross-border trade entails. A non-exhaustive list includes supply chain delays, regulatory drift/surprise, country-specific or political risk, and the risk that physical commodities degrade (see below for dilution risk).
* **Complexity Risk**: “Abstraction” is both a strength and a risk of opportunities which fall under the Arranger model. When applied to a complicated space like cross-border trade, the arranger model may limit visibility into the essence of the risks being incurred. In Untangled’s case, it retains a fairly broad mandate to originate trade finance assets of many ilks. Different geographies, different industries, different risk profiles, different maturities, different default/recovery proceedings, different security guarantees etc. The assets are heterogeneous, ranging from invoices to repos to inventory, making the breadth of the exposure difficult to visualize. Finally, given the long chain of dependencies (Maker → Untangled → Asset Originators → SMEs around the world), assets are located “far away” from MakerDAO.

**Primary Opportunities:**

* **On-Chain Securitization**: From the outset, Manrui and Quan have built their business with RWA tracking and securitization via blockchain as a core pillar. Untangled is committed to exploring the frontier of how [supply chains are refined via tokenization 2](https://medium.com/untangledfin?\_branch\_referrer=H4sIAAAAAAAAA8soKSkottLXz8nMy9bLTU3JLM3VS87P1TfIS3GsKLOICM1KAgB2h5KMIwAAAA%3D%3D). As a mitigant to the aforementioned ‘complexity risk’, Untangled’s digital securitization platform should provide MakerDAO with a degree of transparency beyond that of prior onboardings, unlocking more granular and actionable performance data.
* **Geographical Diversity**: Untangled represents an opportunity to achieve exposure to Africa, the Nordics, Western and Eastern Europe, the Middle East, and APAC, the latter of which will be the economic engine of the world for the next ten years. Given the >85% exposure of committed debt ceilings to US-based credits, exposure to other countries will diversify credit risk and help expand DAIs footprint internationally.
* **Impact Exposure**: Untangled’s roadmap has long since included green bonds as part of the phased roll-out. The principals have expertise in agricultural feasibility and finance in Africa and Vietnam. Further, Quan/Manrui have been receptive to the MakerDAO community’s interest in impact investing and have tailored their asset originator pipeline accordingly. By working intimately with Untangled, MakerDAO will have the opportunity to guide Untangled’s scaling toward asset originators making a dent (as opposed to funding greenwashing).
* **Scale**: Untangled operates in the nitty-gritty supply chain space. Though traditional trade finance is fairly well-supplied, Untangled targets international trade finance which is more focused on cross-border shipments and commodity-heavy industry. The principals’ agricultural and supply-chain centric backgrounds provide an edge in underwriting these credits. With a competitive cost of capital, Untangled has the potential to scale to \~$175MM in two years time. Its onboarding [pipeline 9](https://docs.google.com/spreadsheets/d/1WFeLP6BS6RtJb2SkjmETELI6exnOdwNypsCmu\_HrtYU/edit#gid=0) suggests ongoing negotiations with >8 originators (beyond the initial four) are in motion.

**Consider the following:**

* Does the opportunity add robustness, yield, or strategic exposure to the current collateral base? Or does it represent a downgrade along these dimensions?
* Does the collateral play a strategic role in generating the scaled, diverse, and impact-oriented collateral base for DAI’s future?
* In other words, is the opportunity sufficiently attractive to incur the risks associated with it?

### Outline <a href="#outline-4" id="outline-4"></a>

**1. Industry Analysis**\
**2. Arranger Analysis**\
**3. Key Risks**\
**4. Issuance Platform**\
**5. Implementation Details**\
**6. Structure and Proposed Covenants**

### Industry analysis <a href="#industry-analysis-5" id="industry-analysis-5"></a>

International Trade Finance refers to the issuance of credit, typically via factoring or supply chain finance, to enable cross-border trade. At the core of factoring is a mismatch between a supplier’s working capital needs (i.e. today’s needs) and delayed payment from its buyers. A supplier will sell an accounts receivable to a lender for a discount (a factor) in exchange for immediate liquidity. Alternatively, a buyer may seek to deliver payment for goods or services early to achieve a discount. In supply chain finance, the lender delivers discounted payment to the supplier in exchange for credit exposure to the buyer. Usually the counterparty that faces an international trade finance lender is either an importer (buyer) or an exporter (seller), who will either sell or pledge underlying assets to said lender. In trade finance, the most common form of collateral is an accounts receivable, of which an invoice is a component. Lenders like Untangled may also lend against physical collateral such as an inventory of commodity stock.

Trade Finance is expected to reach a market size of [$11 Trillion as of 2026](https://www.globenewswire.com/news-release/2021/05/26/2236093/0/en/Global-trade-finance-market-anticipating-a-high-boost-at-a-CAGR-of-5-4-during-2021-2026.html). Roughly 80-90% of global trade is reliant on trade finance solutions. Traditionally, a gap has existed between the supply of credit and the demand for trade finance solutions. In 2018, this figure was $1.5 Trillion. Though large commercial banks do supply the space, an underbelly of SMEs remain underfunded, especially in the wake of the pandemic. In 2020, the global trade finance gap ballooned to an all time high of $1.7 Trillion, a [15% increase on two years prior](https://www.adb.org/publications/2021-trade-finance-gaps-growth-jobs-survey). The contraction of trade credit disproportionately affected SMEs, accounting for 40% of rejected trade finance requests, as per the 2021 Trade Finance Gaps, Growth, and Jobs Survey.

More recently, nimbler and more opportunistic credit funds and specialty finance firms are entering the space as credit becomes more accessible and trade activity becomes more complicated. These players typically have a more intimate knowledge of particular sectors within the broad TFA space. However, unlike large banks, credit funds do not have the benefits that come with retail deposits, namely a continuous line of liquidity. Instead, debt funds rely on discrete infusions of capital via equity and debt. Securitization of underlying trade finance assets, particularly if catalyzed by blockchains, can bring ample liquidity and transparency to these processes.

For United States-based trade finance, SMEs can typically access 10-12% financing to meet their working capital needs. However, for companies overseas, particularly those involved in cross-border trade, these rates jump to above 15% (usually closer to 20%). This financing gap presents an opportunity for lenders familiar with the intricacies of international and cross border trade.

**How do the assets respond in the event of a particular major negative economic event?**

Like with any financial asset, a macroeconomic downturn or general contraction in economic activity will increase the likelihood of losses on trade finance loans. Because such loans are secured by promises to pay at some point in the future, defaults anywhere along the chain of credit contingencies can reverberate through to the obligor. Interestingly, as traditional institutions seek to trim exposure to trade finance assets during downturns, specialty lenders and debt funds may see an uptick in new business that may help offset charge-offs on the outstanding book. Further, when crises take hold, self-preserving obligors are loath to renege on the invoices that keep their businesses operational: a business owner will probably explore alternative avenues when implementing an austerity program.

**What remedial measures might be undertaken?**

In trade finance, lenders typically either buy outright (true sale) or hold a security interest in an invoice, purchase order, receivable, payable, or inventory set. In the case of the latter collateral form, a collateral agent will be appointed by the lender to secure, manage, and verify the pledged collateral. Credit insurance may be pursued by asset originators to hedge against the impact of a default by a borrower. Further, in the case that explicit credit insurance is not purchased, guarantees (often from the parent company) offer security. If a default does occur, an asset originator/arranger may opportunistically sell off the impaired note to a third party.

**What are the historical default rates in this industry?**

Trade finance assets have experienced [relatively low levels of default 2](https://iccwbo.org/publication/icc-trade-register-report/#1550486691378-3a223d05-6e5e). Historically, the industry-wide default rate at the obligor level has been .75% for import/export loans and .47% for supply chain finance. At the facility level, these rates improve to .26% and .17% respectively.

### Arranger Analysis <a href="#arranger-analysis-6" id="arranger-analysis-6"></a>

Untangled Finance is an asset manager. In this case, we mean a fund that faces asset originators, as opposed to facing the underlying borrowers/obligors directly. Untangled was incorporated in 2020 by Manrui Tang and Quan Le. Prior to founding Untangled, both Manrui (COO) and Quan (CEO) founded and operated Binkabi, a blockchain-based commodity trading and financing platform. Quan and Manrui are both Chartered Accountants and have a combined 10+ years auditing and performing due diligence on financial institutions.

Binkabi’s supply chain finance solutions were constructed in partnership with a bank and commodity exchange. The platform has rolled out integrations with three banks and two collateral managers. Though demand has been muted due to COVID and the concomitant supply chain issues, the platform has processed 500K metric tons since July 2020. Binkabi launched a supply chain finance (SCF) pilot program with the biggest commodity exchange in South Africa just prior to COVID. Finally, a listed Nigerian Bank has invested $500K in Binkabi via an equity infusion.

The Untangled Finance digital credit fund is a separate vehicle that builds on the learnings/technical know-how achieved during the roll-out of Binkabi. Up Series LLC is an Untangled-operated SPV which faces the originator-operated Asset SPV directly. It will enter Master Note Purchase Agreements with the Asset SPVs created by asset originators. Untangled Finance will execute an engagement letter with the asset originator parent company itself. Please refer to the funding structure in the ‘Implementation Details’ section below for elaboration.

**What is the background of the Arranger’s managers?**

Manrui Tang: After graduating from both Imperial College London and the London School of Economics, Manrui started her career in financial services, doing Mergers & Acquisitions work first for PriceWaterhouseCoopers and then for National Grid, a utility company. Whilst at National Grid, Manrui was involved in the company’s ‘green’ energy transition through investment in smart grid and smart meters. After ten years in M\&A, she founded Binkabi in 2017 with Quan.

Quan Le: Quan also began his career at PWC, where he spent 17 years on strategy, M\&A, and audit. In 2011, Quan founded growmoreX , where he architected and set up rice farms in Africa based on long-standing Vietnamese know-how. Quan [pioneered 3](https://thebreakthrough.org/articles/revolution-in-africa) drone technology in terrain mapping and water engineering in Africa. He worked with large, commercial clients such as Unilever, Diageo, Olam, Stallion, Leventis, IFAD, AfDB, and private equity firms SCPE and Advantage partners. With the help of Manrui, the duo founded Binkabi in 2017.

**Has the Arranger implemented a technical solution to support the onboarding and securitization of assets?**

As a successor to Binkabi, Untangled has funded and built a blockchain securitization platform. The platform is similar to the technical solutions for RWA tokenization that MakerDAO has utilized in the past. A key difference is that Untangled tokenizes trade finance assets (e.g. invoices) at the asset level.

The Untangled platform represents a nexus and single source of truth for all financing participants (originators + investors) to utilize. Asset originators will upload asset pools directly to the platform. APIs specific to the originators will help feed live performance/collections data directly to the platform. The platform accommodates the representation of batches of financings as NFTs. The Untangled digital credit platform translates cash flows into SOT and JOT, the senior obligation token and junior obligation token, respectively.

**Underlying Asset Originators - What is the profile of the credit in the initial pool?**

Untangled has identified four initial asset originators to serve as the pilot cohort for the digital credit fund:

_Fig. 1_

[![P1](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/8/89fab9491843abf5d28a60b729d2349df6e80f44\_2\_690x103.jpeg)P11248×188 42.2 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/8/89fab9491843abf5d28a60b729d2349df6e80f44.jpeg)

**A**: The first is a Singapore-based global invoice exchange. Via this exchange, companies can raise funds by selling discounted invoices to investors. This originator was founded in 2016 and has financed roughly $400MM in trade receivables. Over the 2020-2021 period, this originator secured a combined $27MM in funding from Sequoia Capital and an investment firm associated with the Singaporean government. The back-tested default rate of this originator is \~0.2% which is in line with the industry average. The primary business line is invoice finance and all exposures are credit insured.

**B**: The second is a Dubai-based supply chain finance (SCF) and receivables finance platform assisting GCC SMEs with working capital solutions. The company was formed in 2016 although it debuted its ecommerce SCF business in 2019. Since inception, the platform has executed $16MM of transactions. This originator was acquired in 2021 by a NASDAQ-listed fintech company and has no history of defaults. Though without credit insurance, the platforms upon which its obligors transact, such as Talabat, Zomato, and Amazon preferentially direct proceeds from merchant sales to the lender first. Exposures will be covered through a performance guarantee from the public parent company, which has a $350MM market cap.

**C**: The third, a commodity markets alternative lender, was founded in 2013. It is entering its fifth year of active lending and boasts large pension funds as investors. The firm focuses on three asset types: trade finance, receivables, and [repos 1](https://www.lexisnexis.co.uk/legal/guidance/commodity-repo-transactions-true-sale-considerations). Many exposures are without credit insurance but have guarantees from the parent companies.

**D**: The fourth is a Switzerland-based commodities trading group with a large Turkish subsidiary that is one of the largest wheat importers in the region. Importing wheat primarily from Russia and Ukraine and supplying it to Turkish millers, the subsidiary was formed in 2016 and turned over 590MM USD in commodities in 2020. All transactions are denominated and settled in USD. The subsidiary has recently been audited (Beau HLB Audit) and is in sound financial standing.

**Scaling: What detail has the Issuer provided on its scaling roadmap? Elaborate on the progress the Arranger has made in onboarding asset originators.**

Untangled has provided a [roadmap 9](https://docs.google.com/spreadsheets/d/1WFeLP6BS6RtJb2SkjmETELI6exnOdwNypsCmu\_HrtYU/edit#gid=0) that details its intentions for onboarding underlying asset originators. It estimates the potential for asset participation at $175MM in two years.

Untangled has either an NDA or data room executed with each of these prospective counter-parties. The composition of prospective asset originators represents geographic diversity across Ireland, the UK, Canada, Eastern Europe, the Nordics, APAC, Africa, and the Middle East. As per discussions thus far, the average potential participation for these asset originators is \~$15MM. With a smaller exposure per originator, as the arranger scales, so does the extent of diversification.

If the DAO were to approve Untangled under the [Arranger Model 4](https://forum.makerdao.com/t/the-arranger-model-a-highly-scalable-rwa-framework/11298) for an initial vault, upon satisfaction of/performance on the obligations laid forth under the initial vault, it could “toggle-on” this diversified scaling map.

**What is the due diligence the Arranger applies to asset originators and their assets?**

The Untangled opportunity is an example of the Arranger Model. By this token, Untangled will front load due diligence and monitor collateral exposures on an ongoing basis. This due diligence process incorporates **country, counter-party, and collateral** when conceptualizing risk.

**Country**: Untangled applies a risk score to the jurisdictions from which it may source participations. Certain geographies will simply be excluded due to unpredictable geopolitical environments or harmful regulatory regimes. Exposures to countries in the acceptable risk band will be attenuated as per the geographical concentration covenants (see below for detail).

**Counter-party**: Untangled scrutinizes the asset originator and its industry. The process verifies that the asset originator’s policies, procedures, and historical performance are strong before providing criteria for eligible participations. With specific regard to the originator analysis:

* Experience and background
* Underwriting/scoring
* Origination strategy
* Bad debt experience
* Regulatory licensing
* Auditors, accountants, and lawyers
* Risk monitoring
* Systems and data
* Credit insurance
* Servicing strategy
* Performance reporting
* Collections policies
* Growth strategy
* Financial standing/quality of performance guarantees
* Current funding structure

**Collateral**: The portfolio will target TFA assets with an average exposure of $250K. Untangled requires a complete data room of all loans that have ever been originated on an originator-by-originator basis. It will investigate the nature and quantity of historical bad debt, the drivers of those write offs, and how the originator intends to mitigate such occurrences in the future.

**What is the valuation model used by the Arranger?**

Trade finance assets are valued via a fair value discounted cash flow (DCF). The present values of all assets in a pool, derived by discounting the future expected cash flows of individual TFAs, e.g. receivables, are aggregated to calculate the Net Asset Value, or NAV. This is standard practice in both trade finance and more broadly in the valuation of risk assets with associated cash flows and limited secondary market liquidity.

Untangled’s DCF approach:

1. _Expected Cash Flows_: ECF is calculated based on the A) expected timing of repayments and B) expected payment amounts. This exercise is a simple mapping of the underlying obligors’ contractual obligations.
2. _Risk-Adjusted Expected Cash Flows_: Adjust the expected cash flows with an Expected Loss variable as informed by the obligor’s credit risk. Untangled assigns each exposure a risk class. This exercise tags a probability of default (PD) and loss given default (LGD). Expected Loss = (ECF) \* (PD) \* (LGD)
3. _Incorporation of Expected Loss_: Losses are subtracted from projected contractual inflows
4. _Discounting_: Discount risk-adjusted cash flows by the opportunity cost of capital. This incorporates the time value of money—what an investor may expect to receive on an alternative investment of equivalent risk, scale, and maturity. Each individual asset in a pool will be assigned its own discount rate. Present values on a per-asset basis are calculated. See below graphics for detail:

_Fig. 2_

[![P2](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/1/192719e9effe9b2254f9fa688096f2b098b6bb3b\_2\_690x304.jpeg)P21024×452 47.6 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/192719e9effe9b2254f9fa688096f2b098b6bb3b.jpeg)

1. _Calculate NAV_: Add up the present values to calculate the value, at time = 0, of the entire pool of assets. See notes below for additional adjustments to NAV.

Note: Write-Offs: If an expected payment does not land as per contractual obligations, the required payment may be partially extinguished by a predefined percentage after a predetermined number of days.

Note: NAV will be updated regularly and visible on Untangled’s credit platform (See Fig. 6 for more detail)

**What is Arranger’s risk methodology?**

Untangled uses real-time NAV calculation to ensure that the junior tranche is above the minimum proportion of total asset exposure (in this case 10%). Because the underlying securities do not have a liquid secondary market, NAV is calculated via the aforementioned fair value calculation.

Trade finance assets will be tiered into six categories of risk: A-F. These risk tiering is driven by the expected losses/write offs (i.e. Probability of Default x Loss Given Default). The riskier the participation, the lower the advance rate, the higher the interest rate, and the lower the financing amount. The aggregate risk scorecard of the portfolio of TFAs also drives the Net Asset Value (see previous section for valuation methodology and Fig. 3 for risk tiering)

_Fig. 3_

[![P3](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/f/fbf886d9c1597e2969077ba85475b0bf63912579\_2\_690x353.jpeg)P31280×656 78.1 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/f/fbf886d9c1597e2969077ba85475b0bf63912579.jpeg)

For default probabilities (PD) and loss given default (LGD), Untangled’s projections fall within industry-wide data from Scope Rating and Altradius over a (4 year) credit cycle.

_Fig. 4_

[![P4](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/7/752ba9e445beec3244160e2cd82f6ba36e5568ab\_2\_690x454.jpeg)P41112×732 111 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/752ba9e445beec3244160e2cd82f6ba36e5568ab.jpeg)

_Fig. 5_

[![P5](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/a/a7dadd56738079ac6dbbfe0f4bdf4879e729b08f\_2\_642x500.jpeg)P5972×756 55.8 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/a/a7dadd56738079ac6dbbfe0f4bdf4879e729b08f.jpeg)

**Untangled Base Case**: a probability of default for assets that are 90 days past due of 3 - 5% and loss given default of 50% over the cycle. This maps to an expected loss of 1.5%-2.5% before the application of credit insurance or parent company performance guarantees.

**Bear Case**: Untangled applies a number of stress tests to the portfolio to ensure that the capital stack can endure a series of unlikely events and the associated expected losses:

1. Stress #1: Maximize probability of default
2. Base case: 3 - 5%, Bear Case: 8%
3. Stress #2: Maximize loss given default
4. Base case: 50%, Bear Case: 90%

**In a stressed portfolio scenario, Untangled expects a maximum annual loss of 7.2% (8% PD x 90% LGD) on its total TFA asset base. This expected loss calculation is considered independent of credit insurance and performance guarantees**

**What is the nature of asset defaults for the Arranger, and the possible solutions?**

The issuer, Untangled, may default on its obligations to MakerDAO in the case that a series of exposures take losses simultaneously. This could occur as a result of either a single asset originator becoming insolvent or macroeconomic headwinds causing a wave of defaults at the asset level. Aforementioned risk factors, namely supply chain risk, could aggravate these events.

Upon the occurrence of an Event of Default, the Trustee shall demand that the liabilities become immediately due and payable at their default redemption amount. Events of Default include

1. A payment event of default
2. A non-compliance event of default
3. A bankruptcy event of default

The structure of the participation between Untangled and the underlying Asset Originators is one of True Sale. Non-true sale assets will not be considered eligible for financing via Maker DAO. A True Sale means that the asset originator transfers, sells, and conveys to Untangled 100% ownership in the recourse rights to the underlying assets. In a scenario where the underlying collateral is inventory, a dedicated collateral agent will facilitate foreclosure of the physical assets (usually commodities) in question.

Despite the assumption that international finance is messier from a transit perspective (which it is), from a security and collateral interest (and thus post-default recovery) perspective, it can actually be preferable for a lender. Most goods bound for international transit are represented by a Bill of Lading, or ‘bladings’, a title deed for (mainly) sea-faring goods. Protected by international and maritime law, bladings confer a more robust entitlement to the underlying cargo than airway bills, railway bills, and truck receipts.

As mitigants, covenants are structured such that exposure to any one country, one asset originator, or one asset is pared down. More importantly, 70% of the underlying exposures will be hedged with some sort of insurance.

**How does MakerDAO monitor the portfolio composition? Can the valuation and risk methodologies be verified?**

Untangled intends for its digital credit platform to be an end-to-end on-chain financing solution.

_Fig. 6_

[![P6](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/2/2ae1bb24b1c28a07818d39ce346079acf9318f0e\_2\_690x327.jpeg)P61248×592 106 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/2/2ae1bb24b1c28a07818d39ce346079acf9318f0e.jpeg)

The Net Asset Value of the portfolio is updated regularly and visible to MakerDAO within the Untangled platform. MakerDAO can actively monitor the credit enhancement represented by the junior obligation token. This transparency permits Maker to ensure that both asset originators and Untangled are in fact retaining first loss pieces of the capital stack.

Collections and asset performance are monitored on chain. Assets are short term relative to other Maker vaults so deterioration in the portfolio’s performance can be seen early. Should collections drop significantly, Maker can preemptively cut funding for new participations.

### Key Risks <a href="#key-risks-7" id="key-risks-7"></a>

1. **Execution Risk**: Untangled Finance was launched in August of 2020 and thus does not have a rich history of performance. The principals do not have significant experience in credit underwriting. In conjunction, these factors make it difficult to gauge how successfully the asset manager will either A) Be able to deploy capital at scale and attract reputable credits and B) Monitor the ongoing performance of an asset base spread across geographies, credit qualities, and verticals. The former concern (A) has affected the velocity of MakerDAO vaults in the past.
2. **Alignment Risk**: For non-institutional asset managers/originators, the expectation is for the counter-party to retain at least 5% of the total asset exposure—typically a first-loss piece. Untangled will commit to retaining ½ of the first-loss tranche, or 5% of the total asset exposure on-chain. Untangled will help fund this retention via an equity raise, or LP interests. Limited Partners refer to the passive Untangled investors to whom Untangled has fiduciary and reputational obligations. A non-institutional asset manager just starting out might elect to commit to a larger portion (>5%) of risk-retention to bring comfort to its senior lender.
3. **Complexity**: As proposed, MakerDAO would lend to an asset manager (Untangled) who would source international trade assets, from many originators, of different risk profiles and maturities, across many different geographies/jurisdictions. Some of the collateral would be simpler (e.g. accounts receivables) and some would be messier (e.g. inventory), requiring physical collateral managers and the associated agreements. The proposed structure would necessitate a few layers of SPVs and a dual-ERC 20 token structure. The modularity, heterogeneity, and complexity of such an arrangement will be costly to accommodate, mainly from a legal perspective. Further, the longer the chain of dependencies, the more uncertain the collections in the case of defaults. This uncertainty poses a tail risk for MakerDAO’s balance sheet.
4. **Supply Chain Risk**: Because Untangled is focused on international trade finance, it necessarily has exposure to the complications that cross-border trade entails. Supply chains continue to grow physically longer and to add dependencies along the way. These changes, both the length and segmentation of chains, have been adopted for the sake of efficiency. But as the pandemic made evident, efficiency can come at the cost of resilience. Many of the asset originators to whom Untangled has exposure will utilize credit insurance to mitigate these concerns.
5. **Commodity Transformation/Dilution Risk**: Dilution refers to any non-cash reduction in a receivable balance that is not attributable to default or write-off. Dilution may occur when the end product or service has somehow deteriorated in quality or quantity. In trade finance, a buyer who receives a product that is different from the one that was conveyed will seek discounting on payment. Typically, in a case where this type of dilution is present, it is the exporter who bears the risk of partial payment. However, in the case of trade finance, this risk is transferred to the asset originator advancing funds today for payment in the future. Dilution may materially impact the collections of the asset originator who advanced dollars. This risk is particularly prevalent in the shipment of non-durable or perishable goods. A commodity may, for a variety of reasons, degrade en route. Upon delivery of a divergent good to the end buyer, the buyer will elect to pay a discount to the seller’s stated accounts receivable or invoiced amount. Often insurance for the goods can mitigate this risk.
6. **Commodity Price Risk**: Both FX risk and commodity price risk are present. The former refers to the risk that the currency an invoice is denominated in loses value over the course of repayment. The latter refers to volatility in commodity prices. Falling commodity prices may undermine the value of inventory-based collateral or constrain a commodity-based business’ ability to perform loan obligations. Rising commodity prices may inflate corporate cost structures, constrain working capital, or cause buyers to renege on unhedged contracts. Some of the asset originators to whom Untangled has exposure will utilize short positions in futures to hedge out price/commodity risk.
7. **Country Risk**: To the extent that a shipment passes through or is destined for a country with a domineering or volatile administration, goods may be seized or delivery delayed.

**Mitigants/Protections - What hedges against the various risks to trade finance will be utilized?**

**Non-Performance Risk**: 70% of the exposures sourced via asset originators will be hedged, either via credit insurance or performance guarantees. Guarantees will only be considered as viable alternatives to de jure credit insurance if the parent company/guarantor has robust financial standing. Untangled always has access to the audited accounts of potential originators. MakerDAO and thus Untangled will regard performance guarantees as legitimate protections in the case that:

1. (Parent Co. Balance Sheet/Debt Service Coverage) is sufficient. For example, in the case of Asset Originator D, the ratio of the parent company’s assets to the debt ceiling allocated to the originator is 20x. (See ‘Proposed Covenants’ for more details)
2. Parent company is listed
3. Parent company is rated as part of a public issuance

**Commodity Transformation Risk**: Cargo, inventory, and warehouse insurance.

**Commodity Price Risk**: By virtue of the short durations of TFAs, price risk is only so relevant. Adverse price movement of underlying commodities can be hedged with futures. This is especially germane to asset originators C and D who traffic in commodities/physical inventory.

### Issuance platform analysis <a href="#issuance-platform-analysis-8" id="issuance-platform-analysis-8"></a>

This opportunity will utilize the Untangled digital credit platform to tokenize TFAs and to track collections/performance.

**Asset Origination and Monitoring Visualization**

_Fig. 7_

[![P7](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/3/3b7e06672a58eaf17fb7739556a343debd337bec\_2\_690x321.jpeg)P71152×536 90 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/3/3b7e06672a58eaf17fb7739556a343debd337bec.jpeg)

### Implementation details <a href="#implementation-details-9" id="implementation-details-9"></a>

**Funding/Organizational Structure**

_Fig. 8_

[![P8](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/1/172814aca61414dac5d8bea03c680e7ba128d73e\_2\_690x320.jpeg)P81248×580 100 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/172814aca61414dac5d8bea03c680e7ba128d73e.jpeg)

The Untangled securitization and marketplace platform will be used exclusively to facilitate the onboarding and monitoring of the TFAs submitted by various Asset Originators.

1. Asset Originators, upon acceptance of a term sheet, will upload asset pools and connect data APIs to the Untangled platform. These assets will be subject to a standard trade finance asset [master participation agreement.](https://docs.google.com/document/d/1e0yiXC3X75FyyIG0IKg0hFP\_4M-1UgvV50pBC8Wn-Qg/edit) The standard BAFT template for English law utilizes a “true sale” of the underlying assets.
2. The platform will enable the automation of or at least standardization of legal contracts and will transmute promissory notes to NFTs. This supports the tokenization of the underlying cash flows.
3. Once pools are operational, the securitization platform allows MakerDAO and other investors to granularly “look through” to the asset behavior. This increased transparency supports monitoring and early triggers that augur degradation of the underlying.

_Fig. 9_

[![P9](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/a/a3ccba91d131a226b6bf1b2ef9b389f3760c9a0a\_2\_690x395.jpeg)P91236×708 90.9 KB](https://makerdao-forum-backup.s3.dualstack.us-east-1.amazonaws.com/original/2X/a/a3ccba91d131a226b6bf1b2ef9b389f3760c9a0a.jpeg)

The above diagram outlines the structure for implementation with Untangled. The on-chain risk retention by Untangled will be 5% of the total debt exposure in the form of JOT ownership. This retention will be visible on-chain. Asset originators will retain a minimum of 5% of the exposure at the asset SPV level—also via JOT ownership.

### Structure and Proposed Covenants <a href="#structure-and-proposed-covenants-10" id="structure-and-proposed-covenants-10"></a>

Such covenants are soft covenants and do not automatically trigger liquidation proceedings.

* Untangled’s credit facilities to asset originators will advance a maximum of 95% against the purchase price of the underlying TFAs.
* Outstanding exposure to any single asset originator’s asset base will not exceed ⅓ of the total debt ceiling, either today or in the future (barring signal requests).
* The net outstanding loan dollars to obligors in any one non-USMCA, non-EU nation will not exceed ⅓ of the total debt ceiling
* Outstanding exposure to any single TFA asset will not exceed 5% of the total debt ceiling.
* Outstanding exposure will be 70% insured against non-performance. This coverage will be achieved by either credit insurance or performance guarantees (should the parent entity qualify).
* For performance guarantees from parent entities to be considered legitimate, parent entities must either:
  * A) Be publicly listed
  * B) Be rated as part of a public issuance
  * C) Have an asset/allocated DC ratio of > 10X

### Allowed investments <a href="#allowed-investments-11" id="allowed-investments-11"></a>

List the kind of investment that the SPV can make. Try to be as specific as possible.

* Trade finance assets backed by either invoices, inventory, or revenue.
* Trade finance assets that have been conveyed to Untangled under a True Sale Agreement
* Maximum maturity of 120 days
* Asset Originators with a minimum of three years of operating history
* Asset Originators with T-12 annual volume in excess of $50MM AND at least two years of profitable operating history
* Untangled is requesting a debt ceiling of 20MM DAI for its first pool. Because the managers will need flexibility to launch effectively and onboard low-risk credits, MakerDAO is not requesting any express allocation towards green or impact investments for this first pool. The Maker community will likely elect to make debt ceiling increases contingent upon allocation towards impact credits.

**Maximum Advance Rate: what % can Untangled advance against the value of the underlying trade finance assets?**

(Loan Amount Per Asset/Purchase Price Per Asset) = 95%

Detail: In factoring, for example, the Asset Originator will purchase an Invoice/Accounts Receivable with a 30-day term from a seller for a discounted price. A maximum advance rate of 95% allows Untangled to participate in $95 of each $100 of underlying TFAs.

**Asset SPV Credit Enhancement**

5%

Detail: Asset Originators will retain a minimum of 5% of the asset exposure at the asset SPV level. See Figure 5 above for visualization.

The first-loss tranche, or equity tranche, of the Asset SPV (or the vehicle operated by the asset originator), will be 5% of the NAV of the TFA assets purchased. This 5% buffer will protect the exposure of the Maker vault.

Asset SPV Credit Enhancement = (Asset Originator Retained First-Loss Exposure/NAV of Participations Held in Asset SPV)

**Minimum Maker Vault On-Chain Credit Enhancement**

5%

Detail: Untangled will retain a minimum of 5% of the exposure to the NAV of UP Series LLC SPV participations. This will be achieved through retention of a first-loss tranche that is junior to on-chain senior positions, both those of Maker and other senior co-investors. Untangled will demonstrate this alignment by holding JOT.

**Minimum Maker Vault Collateralization Ratio**

100%

**Maker Vault All-In Maximum LTV**

To visualize the protection for the Maker Vault, consider the following cushions:

* Advance Ratio: 95%, 5% cushion
* Asset SPV Credit Enhancement: 5% cushion
* Maker Vault On-Chain Credit Enhancement: 5%
* Maker Vault SOT Overcollateralization Cushion: 0%

Maker Vault All-In Maximum LTV = (Advance Ratio) \* (1 - Asset SPV Credit Enhancement) \* (1- Maker Vault On-Chain Credit Enhancement) \* (1 - Maker Vault Overcollateralization Cushion)

Maker Vault All-In Maximum LTV = (95%) \* (100% - 5%) \* (100 - 5%) \* (100% - 0%) = 85.74%

Reframing, the Maker Vault All-In Overcollateralization = (1/.8574) = 116.63%

**If each asset that Untangled participated in represented the maximum 5% of the total debt ceiling, this LTV would permit the concurrent default AND 100% Loss Given Default (LGD)/complete write-off of \~3 assets without incurring a loss. The likelihood of such an occurrence is very low:**

1. The industry-wide default rate at the obligor level has been [.75% for import/export loans and .47% for supply chain finance 2](https://iccwbo.org/publication/icc-trade-register-report/#1550486691378-3a223d05-6e5e).
2. Untangled and each Asset Originator hold 5% first loss positions in the assets. Untangled is thus incentivized to fund assets in a more diversified, granular way. If it were to fund a single asset at the maximum concentrations (5% of total debt ceiling) and this asset were to be completely unrecoverable, Untangled would eat the loss.

In order to monitor the real-time collateralization, the Untangled platform provides MakerDAO with daily valuation updates on the assets in which it has participations. Untangled will also provide a projected and active non-performing loan (NPL) report on a monthly basis. The active portion will detail delinquencies, expected loss amounts per asset, write-offs, and remedial/collections strategies. This section will include detail on participations/notes that are opportunistically sold off to external investors at discounted rates. The projected portion will be informed by a series of leading risk indicators. The NPL report will track actively delinquent exposures and how cash flow recovery is progressing. In order to monitor real-time collateralization and concentration risk. Untangled will provide to MakerDAO:

* Daily NAV calculations: risk-adjusted DCF + write-offs
* Concentration matrices monthly
  * Geography
  * Asset type (i.e. inventory, invoice, repos)
  * Asset originator

MakerDAO further expects complete documentation on participations (e.g. Master Agreement), proof of insurance/parents company guarantees, and true sale execution.

### Concentration risks <a href="#concentration-risks-12" id="concentration-risks-12"></a>

* Exposure to any single asset originator’s asset base will not exceed ⅓ of the total debt ceiling, either today or in the future (barring signal requests).
* Exposure to obligors in any one non-USMCA, non-EU nation will not exceed ¼ of the total debt ceiling.
* Exposure to any single TFA asset will not exceed 5% of the total debt ceiling.

### Stakeholders rules <a href="#stakeholders-rules-13" id="stakeholders-rules-13"></a>

The risk team has not been provided with access to the counter-party’s financials. Without this visibility, it is difficult to make a determination on the likelihood of solvency/continued operation on a 12 month time scale. The ultimate term sheet and vault will, of course, be contingent upon satisfactory evidence of financial health. Please see the below attestation from Untangled’s founders:

“As you know we are a start up and our pool is not live. We have however invested heavily in technology and business development with founders’ and angels’ equity. We are in the process of venture fundraising so it is fine to include the financial as a condition precedent for vault disbursement. We are confident that by the time our \[risk assessment] is approved we will be able to provide the required proof for the junior tranche. We have every interest to make this partnership a success.”

**The proposed structure in regards to alignment is as follows:**

* All first-loss and junior exposure will be visible and verifiable on-chain
* Asset Originators (one level beyond Untangled) will retain 5% of the exposure to underlying obligors at the Asset SPV level.
* Untangled will retain at least 5% of the total debt exposure. This 5% will be raised via solely LP commitments.
* Untangled and the underlying asset originators will realize losses and cash flows to the junior tranche on a pari passu basis. In other words, within the junior tranche, neither party is junior to the other. Losses and gains are distributed to both parties on equal footing.
{% endhint %}
