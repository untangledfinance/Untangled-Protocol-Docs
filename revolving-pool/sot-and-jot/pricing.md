# Pricing

As the Pool is revolving it continuously receives new subscriptions and makes redemptions until the Term Length is over or the notes are fully redeemed. In the absence of a secondary market for SOT and JOT, their pricing has to be determined by the Protocol, based on such factors as the terms of the notes, Yield to Maturity and NAV Calcs. The Protocol will quote the price of SOT and JOT on a live basis to allow Liquidity Providers to subscribe or to redeem.![](https://lh3.googleusercontent.com/ruDw1e6l7yyu4x7Gzx6NTP7hMZnutNLBFFxEe0TFsrtSS2M\_DGcxdlRePZ\_V88FyuIsbBajrDgCw6HBG6txwS0UsMhRnCOGJLGcjzG8ewc5bN-EQzMa2OwJ8-g7\_rQ-IREuBzwQl)

SOT Tranche Value = Max (Bond pricing formula with coupon compounded by second (APY) and Yield as inputs, NAV)&#x20;

SOT price: SOT Tranche Value / Number of outstanding SOT&#x20;

If NAV <= Senior Tranche Value then Senior Tranche Value = NAV&#x20;

When this happens, Junior Tranche Value will go to zero. In other words, when Assets are not performing, NAV will decline which will first wipe out the Junior Tranche (therefore it is first-loss) before the Senior Tranche is being affected.&#x20;

`JOT Tranche Value = (NAV + Reserve) - SOT Tranche Value`&#x20;

`JOT Price = JOT Tranche Value / Number of Outstanding JOT`

