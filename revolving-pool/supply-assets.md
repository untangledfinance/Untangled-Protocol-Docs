# Supply Assets

## Agency Origination model&#x20;

Approved Originators can sell Assets to the Pool (referred to as True Sale in CeFi) or pledge Assets to the Pool in order to borrow from the Pool Reserve. Note that the Protocol does not explicitly support Asset Purchase Agreement but this can be arranged off-chain between Issuer and Originator. As part of the process of creating a Pool, Issuers can define an onchain risk scorecard which classifies Assets into 5 groups A, B, C, D, E, F depending on their asset quality. The Asset Purchase Agreement mentioned above could define the classification criteria such as days past due. The risk scorecard will be used to price the Assets being sold to the Pool (called Advance Rate) and on-going Net Asset Value Calculation. Refer to the technical specifications of the risk scorecard.

### Net Asset Value Calculation (NAV Calcs)&#x20;

The revolving nature of the Pool means that Liquidity Providers can subscribe or redeem the Senior Tranche token at any time as long as there are available funds in the Pool Reserve. Net Asset Value Calculation is based on the Discounted Cash Flow (DCF) method. DCF is used because there are no secondary markets for loans. The Protocol uses Day Past Due as a proxy to asset quality. Each Asset is allocated a risk core which varies daily based on the past due status. Each risk score corresponds to a Probability of Default and Loss Given Default. From this, Expected Loss (EL) is calculated:&#x20;

`Expected Loss = Probability of Default x Loss Given Default`&#x20;

`Net Asset Value = Present Value of Cash Flows from Assets - Expected Loss Asset`&#x20;

### Repayments&#x20;

As the Pool contract owns the Asset NFTs (LAT, AIT) it will receive any repayment relating to those Assets. Anyone (Borrower or Originator) can call to repay using the token ID and the repayment amount will be routed to the Pool.
