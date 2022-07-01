# More on liquidity and liquidation

{% hint style="info" %}
Thank you for posting this thoughtful summary - very useful! It’s also great to see that you mention the legal challenges around tokenizing RWAs, looking forward to learning more about your approach with Untangled.

Regarding the liquidity-impact tradeoff, I spent some time thinking whether a tiered liquidity setup would help. On a high level, it could work something like this:

* We (logically) split the reserve into a core reserve and an impact reserve
* The core reserve holds highly liquid assets (e.g. the current crypto assets) and has sufficient collateral to cover all outstanding cStables.
* Let’s define two collateralization thresholds for the core reserve x and X with x < X, let’s say x = 1.5C and X = 2C where C = USD value of stables in circulation, i.e. we aim for 150%-200% overcollateralization with the core reserve (numbers are just examples, TBD)
* If the core reserve value R exceeds X, the difference R-X is ‘transferred’ to the impact reserve and invested e.g. in real world assets
* As long as x < R < X, the impact reserve is not touched
* if R falls below x (trigger event), impact reserve assets are liquidated to boost the core reserve

Would love to hear your thoughts on this
{% endhint %}

We also think the x\<R\<X framework is a good starting point. It has been tried and tested with protocols such as Maker. We call X collateral ratio and x liquidation ratio. By definition x should be more than 100% as we would need to provide some incentive, essentially a discount to ‘fair value’ of underlying assets, to enable a quick sale during a liquidation event.

If cStables are collateralised by crypto natives then there is plenty of data within the Celo network and other similar protocols to model the value of x, X. The UST debacle reminds us of Black Swan events even though, strictly speaking, it was an undercollateralized (algorithmic) stablecoin that was built on an unsustainable foundation.

**if R falls below x (trigger event), impact reserve assets are liquidated to boost the core reserve**

As R fluctuates with underlying crypto collateral and the value of cStables in circulation, boosting R through liquidating impact (RWA) assets could be problematic. Typically RWAs can’t be liquidated quickly but celo could employ a combination of strategies:

1. Creating a safety margin: say liquidity need for a time horizon of 1 week, when the most liquid RWA can be liquidated
2. Creating a liquidity strategy within the RWA portfolios: essentially making conscious tradeoffs among the impact/liquidity and yield
3. Working with real world asset funding protocols to create highly liquid exposures to impact assets

1 above could be implemented with the value of the Celo token in the treasury. However it is much more sustainable to use protocol profits or surplus to fund safety margins. For this reason, celo needs to consider assets yields when making asset allocation decisions.

2 above has been covered in this post. Again all three properties and their tradeoffs should be considered.

3 above starts with selecting quality assets to form the impact reserve. The asset onboarding process needs to follow good practices as being proposed in this [thread 2](https://forum.celo.org/t/discussion-initial-proposal-reserve-asset-onboarding-process/3698/7). It is important to note that once the asset has been onboarded the on-going monitoring is robust enough to ensure all asset risk parameters are in check. Having real/near real-time, on chain asset tracking, net value calculation and reliable oracles is crucial.

Even AAA assets have a non-zero probability of default. A proposer of impact assets (to be included in the reserve) needs to have a pre-approved liquidation process. Typically, these assets are sold under ‘true sale’ to a Special Purpose Vehicle (SPV) whereby an independent administrator or trustee is instructed to liquidate the assets (perhaps with the help of a professional liquidator) when certain conditions are met. This sort of liquidation procedure is well functioned within traditional finance/securitization. The challenge here is to create a legal structure that can work with a DAO as a DAO may not have a legal status.

Legally speaking, impact asset tokens come in two main forms:

* token representing a claim on the actual impact asset
* token representing a claim on the proceed of the impact asset in the event of a liquidation

Both of these are securities: equity in the former and debt in the latter. An equity token might be subject to registration with various authorities before being included in the reserve. Price discovery would need to happen on a licensed secondary market, and in the US, subject to various transfer restrictions. There is also an issue regarding custody of the token, establishing a control location for sovereignty over the custodied token and compliant liquidation mechanism.

Under the second form, assets would be sold to an SPV in the manner described above. Each of the assets are tokenized as an NFT with adequate metadata to enable oracles to price assets on an ongoing basis and in the event of a liquidation. This second form is arguably simpler as it involves less parties, at least in the US. The liquidation process is still manual as described above.

**Solving for the trilemma of impact tokens**

Both of the above are securities so unless they are registered or exempted and listed there are no secondary markets in DeFi. What if there is a token with exposure to underlying impact assets but are not subject to securities’ restrictions? This token would then be traded freely on DEXes such as Uniswap.

This could be done by separating between Liquidity Pool and Asset Pools. Under this construct, liquidity providers would deposit their funds into Liquidity Pool and receive an LP token in return. A permissioned asset originator would sell/upload their asset NFTs to an Asset Pool (a smart contract) to which Liquidity Pool automatically allocates funds under certain conditions.

Liquidity providers can timelock their LP tokens to receive extra allocation of LP tokens and a governance token. The payment waterfall of Liquidity Pool would follow the timelocking of LP tokens e.g., no time lock/immediate, maturing in 1 month, 3 months, 6 months etc. With a suitable design, these time locked LP tokens can follow the ERC20 format, making them composable with the rest of DeFi. A secondary market for these tokens e.g. pairs of LP token/timelocked LP tokens could be enabled.

Neither the Liquidity Pool nor LP token holders are lenders of record. The Liquidity Pool participates in the economics of Asset Pools by virtue of the protocol design (i.e. the smart contract). This would be a leveraged and structured product and in normal financial services the dealer managing this would be regulated. But if the entire mechanism is automated and controls are at the end points - at the originator validation/auditor node and investor onboarding nodes - the internal mechanism can be completely DeFi.

If cStables reserve holds the above LP tokens, not only it is exposed to underlying impact Asset Pools, it could quickly sell the LP token on any DEX when needed. If the LP token also provides yield this could be a solution to the impact asset trilemma.
