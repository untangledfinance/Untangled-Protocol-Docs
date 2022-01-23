# Add Liquidity

To borrow from SOT noteholders, the Issuer first needs to get enough support from JOT noteholders. Let’s say an Issuer wants to raise $1m and the Minimum first loss ratio is 10%, the Issuer needs to raise $100k from JOT noteholders before raising $900k from SOT noteholders. In other words, the amount of leverage (Leverage Ratio) is a multiple of the amount raised from JOT noteholder:

* Target Amount: currency amount to be raised&#x20;
* Term Length: Financing duration&#x20;
* Start Date: the date on which the term starts&#x20;
* Trustee: Trusted independent third party acting on behalf of noteholders

For senior tranche there are two other variables: `Interest Rate` and `Yield`. Interest Rate is the fixed coupon that senior tranche token (SOT) will pay out and Yield is Yield to Maturity, an input to calculate the price of SOT. We will come back to Yield in the later section.&#x20;
