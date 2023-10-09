# NAV calculations

Untangled pool valuation for trade finance assets (NAV)

**Introduction**

Asset Valuation is the process of determining the current worth of an asset or portfolio by assigning a monetary value. The value of a portfolio of assets is often also expressed as the net asset value (NAV).

A NAV is usually required when a portfolio is sold or when investors want to join/exit an existing pool. Then the portfolio value ultimately determines the investment/redemption price. Note that for these purposes the portfolio value may be different to the book value or accounting value of a portfolio.

Determining the value of illiquid assets is difficult because – by definition – there isn’t a liquid secondary market to determine the value, unlike many stocks, bonds or most fungible tokens. For illiquid asset portfolios the valuation methodology is thus often based on a fair value valuation utilizing a financial model. This often comes down to valuing the present value of future cash flows expected to receive based on these financings under discounted cash flow (“DCF”) method.

**Fair value DCF**

1. **Derive Expected Cash flows:** For every outstanding financing (tokenised amount) of an asset, the expected cash flow is calculated. The current implementation allows to calculate the Expected Repayment of simple bullet loan structures which are common in invoice financing and trade finance. The Expected Cash Flow is calculated based on (i) the expected repayment dates and (ii) the expected repayment amounts. (i) The expected repayment date is derived on contractual obligations associated with the financing, e.g. the due date of the underlying asset. This is provided through an daily API call (oracle) for each NFT minted on Untangled Platform. (ii) The expected repayment amount is projected based on the outstanding UP financing by applying the financing fee on the current debt until the repayment date.\

2. **Risk-adjusted expected cash flows**: The expected Cash Flow is risk-adjusted for credit risk by the Expected loss. Every financing is allocated a risk class that has a Probability of Default (PD) and Loss Given Default (LGD) assigned to it. The Expected Loss is calculated as Expected loss = Expected Cash Flow \* PD \* LGD and subtracted from the expected repayment amount to adjust for credit risk. Note that PDs are often communicated per annum and may need to be adjusted to the term of the underlying asset.\

3. **Discount risk-adjusted expected cash flows:** The risk-adjusted expected cash-flows are discounted with an appropriate discount rate (this depends on asset class and pool) to derive the present value of a financing. The discount rate usually reflects the rate of return an investor could earn in the marketplace on an investment of comparable size, tenor and risk. Note that the discount rate is the same for every financing of a pool. The standard formula to calculate the PV of a cash flow is

$$
PV = CF/(1+r)^t
$$

with r = discount rate and t = period of cash flows. As we deal with intra-year cash flows, the formula becomes

![](<../.gitbook/assets/image (2).png>)

4. **Calculate NAV:** Adding up the present values of the risk-adjusted expected cash flows for all financings in the pool leads to the (portfolio) NAV. The NAV plus the liquidity currently in the Reserve of the Pool gives the Pool Value.​

**Write-offs**

If a financing is overdue the expected repayment amount can be (partially) reduced by defined percentages after a defined number of days following predetermined criteria (e.g. a grace period and collection period).

**Operational costs**

Average loan maintenance/running costs (such as legal, SPV, servicing) could be subtracted from the PV.&#x20;
