---
description: Original article published by Muntangled on Celo forum
---

# Green assets as collaterals for stable coins

Collateralised stable coins need to be overcollateralized with quality, stable and liquid assets. In the case of Celo’s stable-coins (cStables), there is a [desire](https://forum.celo.org/t/celo-and-regenerative-finance/1447) to include nature-based assets in the reserve backing up cStables. This post discusses a range of green assets (which include nature based assets) according to their properties: impact, liquidity and yield.

**Green assets’ trilemma - Choose 2 out of 3: impact, liquidity or yield**

[1332×924 28.7 KB](https://global.discourse-cdn.com/standard11/uploads/celo/original/2X/4/4309a829f79bf3d5a89a7b41c514f08ac11ea7e8.png)

![](https://global.discourse-cdn.com/standard11/uploads/celo/optimized/2X/4/4309a829f79bf3d5a89a7b41c514f08ac11ea7e8\_2\_434x299.png)

Impact against climate change: is the impact high and transparently measured? A rainforest offers both a high impact against climate change and an ease of measurement (e.g via satellite or drone survey). On the other hand, the impact of a themed bond issued by a corporation is arguably lower and more difficult to measure.

Liquidity: Is there a liquid secondary market whereby the assets can be sold without affecting its price? A share in a listed renewable energy company (yieldcos) is more liquid than a rainforest in the example above.

Yield: Is the asset offering yield? This is financial yield as the impact referred to above can be considered to be environmental yield. A green bond issued by a corporation offers tangible financial yield compared to a nature-based asset such as peat land.

Based on empirical evidence (see more in the table below) there are trade-offs among impact, liquidity and yield. There are no assets that can fit all three criteria i.e. high impact, high liquidity and also high yield. For this reason, there is a concept called [greenium 4](https://www.climatebonds.net/2021/09/greenium-remains-visible-latest-pricing-study) within the green bond market - given the impact that green bonds supposedly bring, investors have been willing to accept lower returns (yield) in exchange for impact and liquidity.

To be included in the cStables reserve assets will first need to be tokenized. The process of tokenizing a green or a nature-based, real-world asset requires not just creating a token but also a legal representation of the asset. This is something that real world asset tokenisation protocols such as Untangled focus on.

**Classification**

The following green assets are classified according to their corresponding properties. These are based on empirical observations and not theoretical possibilities. They are also investable assets that could, in principle, form part of cStables reserve. The list is not exhaustive so the community can add more.

| ReFi/Green Assets                                         | Impact | Liquidity | Yield |
| --------------------------------------------------------- | ------ | --------- | ----- |
| Solar and wind energy “yieldcos”                          | H      | H         | L     |
| Operating renewable energy projects developed markets     | H      | M         | L     |
| Renewable energy construction loans in developing markets | H      | L         | H     |
| Green receivables such as home solar systems              | H      | L         | H     |
| Natural assets such as REDD+ natural schemes              | H      | L         | L     |
| Green supply chain receivables                            | M      | M         | M     |
| Green bonds                                               | H      | M         | L     |
| Carbon Credits                                            | H/?    | H/M       | M     |

The above assets can be classified further by their functions or instruments:

Function: in terms of CO2 emission, there are nature based assets such as forests or regenerative agriculture land that are good at CO2 sequestration whilst renewable energy assets such as hydro, wind or solar are good at preventing further CO2 emission to the atmosphere. We believe that cStables should be backed by both of these functional assets.

Instruments: The above functional assets can back different instruments such as private credits, listed bonds or equities in renewable energy companies. Depending on the instrument, the impact of the assets might be more difficult to verify. For example, a debt instrument issued by a SPV whose assets are solar home systems in Africa could be easier to verify in terms of impact compared to, say, an ‘use of proceed’ bond issued by a large corporation where there is a lack of transparency on the impact measurement.

Carbon credits are a special asset whereby the impact is highly dependent on the quality of the underlying project. It is arguably more liquid as its trading is more of a ledger entry rather than a complex change of legal ownership often associated with other nature-based assets. Its yield or gain is determined by supply and demand, other things being equal. In the current environment, supply tends to be lower than demand creating an upward pressure on prices. Since there is no such thing as a unified carbon credit, there is no single price for it. This creates a further challenge to impact or quality verification for carbon credits. Further, if carbon credits are meant to be retired and not speculated then an increase in prices might not be desired especially from a perspective of a buyer who needs to offset their CO2 emissions.

**Liquidation**

Onboarding real-world assets to cStables reserve introduces a new risk dimension: credit/counterparty risk. Not all assets will be repaid when due or it is not easy to liquidate them given a lack of a secondary market. Tokenization in itself does not significantly change the liquidity of an asset.

That’s said, some assets are self-liquidated. For example, green supply chain receivables hived off in an SPV could be both short term (e.g. more liquid) and self liquidating. When a receivable such as an invoice becomes due, the invoice receiver/buyer usually pays. In the context of a supply chain it is important to keep your suppliers happy by paying on time so there is no disruption to your business.

For other types of assets, liquidation is necessary when there is a trigger or a breach of covenants. It is important therefore to track the assets beyond the point of tokenization. Having reliable oracles (centralised or decentralised) is crucial in ongoing net asset value calculations (NAV calcs). When the assets are to be liquidated they often follow standard procedures within existing securitisation structure e.g. The Trustee instructs a predetermined liquidation agent to sell the assets and return the proceeds to the reserve or token holders.

Since a DAO may not have a legal status, formalising off chain real-world legal agreements represents unique challenges. Legal structures could be set up to facilitate this. Celo could also learn from other DAOs such as MakerDao.

**Asset allocation strategy for cStables reserve**

Understanding the tradeoffs among the properties of green/impact assets is important in reserve asset allocation strategy. Unlike crypto native assets, these real-world assets are not correlated with the rest of crypto but they are subject to different types of risks such as liquidity and credit risks. Extensive stress testing and backtesting are needed to construct an optimal basket of collateral assets backing up cStables.

Onboarding assets, particularly unlisted assets to the reserve, requires strict procedures. We are therefore welcome onboarding policy discussion as in the [article 3](https://forum.celo.org/t/discussion-initial-proposal-reserve-asset-onboarding-process/3698).

{% hint style="info" %}
**Good to know:** depending on the product you're building, it can be useful to explicitly document use cases. Got a product that can be used by a bunch of people in different ways? Maybe consider splitting it out!
{% endhint %}
