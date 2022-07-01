# Pricing of SOT and JOT

Pricing of SOT and JOT As Asset Pool is revolving it continuously receives subscriptions and makes redemption to Funders until the Pool’s term length is over. In the absence of a secondary market for SOT and JOT, their pricing has to be determined by the Protocol, based on such factors as the term length of SOT/ JOT, Yield to Maturity and NAV Calcs. The Protocol will quote the price of SOT and JOT on a live basis to allow Liquidity Pool to subscribe or to redeem.

![](https://lh6.googleusercontent.com/icVGHIQzSJyfW0QmN6iPCS2ajQMe5l7L38i1NUloUd8n4Za42KRRd7g9U4ofjome-OShtt\_BV75PmFpvbxbFgheA7a9wdN5p62RXAbVU9YcRdQlq1SX3e26oXBbjdu50l6SX6s87RhzLXntnJQ)

SOT Tranche Value = Max (Bond pricing formula with coupon compounded by second (APY) and Yield as inputs, NAV) SOT price: SOT Tranche Value / Number of outstanding SOT If NAV <= Senior Tranche Value then Senior Tranche Value = NAV When this happens, the JOT price will go to zero. In other words, when Assets are not performing, NAV will decline which will first wipe out the junior tranche (therefore it is called the first-loss tranche) before the senior tranche is being affected. JOT Tranche Value = Pool Value - SOT Tranche Value JOT Price = JOT Tranche Value / Number of Outstanding JOT
