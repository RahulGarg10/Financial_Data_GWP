# Financial_Data_GWP


**Introduction**

In lending of any asset or loan and  determining appropriate rates like default probability, credit spread, interest rate, recovery rate etc, we need the 5 Cs (Capacity, Capital, Character, Collateral and Conditions) about the borrower. While in lending securities, the collateral, capacity and character is not of that importance as counterparty risk is mitigated by the exchanges and trading platforms. But giving unsecured loans, information about the capacity and character of the borrower becomes paramount in order to avoid losses. Along with it, we need to be aware of magnifying risks such as leverage & non linearity and frictional challenges like liquidity and regulation. These factors make it important to assess the debt and assets of borrowers and our risk appetite for obtaining a certain amount of returns so that principal is adequately recovered in case of default. Further, we will look for the effect of these factors in student loans as unsecured loan, construction loans to Jones Lang LaSalle Incorporated (JLL), a construction company and Colgate-Palmolive Company (CL), a consumer goods company. This time we will check leverage ratios and solvency ratios of borrowers of both types of loans and effect of credit score on interest rates in case of student loans. In case of security lending, we will assess SPDR Portfolio Corporate Bond ETF (SPBO) and Google (GOOG) stock on expected returns, risk and leverages.


**Data Source**

The data for lending an unsecured loan (Student loans) comes from Consumer Financial Protection Bureau (CFPB) and Federal Reserve Bank of New York (FRBNY) in the form of datasets in excel file and is from 2010-2018 and 2003-2022 respectively. The data for a construction loan comes from FRED and Yahoo finance in the form of rates and balance sheets respectively.The data for both bond and stock also comes from Yahoo finance.


**Now we will assess various lending scenarios on the factors discussed above:**


**1: Magnifying Risks**


|**Scenario**|**Leverage Challenges**|**Non-Linearities Challenges**|
| :- | :- | :- |
|**1\. Unsecured Loan**|<p><ul><li>The borrower already has too much debt compared to assets, which may lead to default.</li></ul></p><p><ul><li>In the case of student loans, the employment outcome is leveraged.</li></ul></p>|<ul><li>The payoff or full payment of principal depends upon the earnings outcome of student or profit exceeding debt taken by the borrower. So, behaving like an option on equity.</li></ul>|
|**2\. Construction Loan**|<p><ul><li>The borrower already has too much debt compared to assets, which may lead to default.</li></ul></p><p><ul><li>The constructed property will have leverage because it is financed by loan.</li></ul></p>|<ul><li>The payoff or full payment of principal depends upon the total debt not exceeding total assets or equity exceeding debt taken by the borrower. So, behaving like an option on equity.</li></ul>|
|**3\. Equity**|<p><ul><li>The borrower may take on too much leverage, which could lead to a default.</li></ul></p><p><ul><li>High-frequency trading strategies have implicit leverage challenges.</li></ul></p>|<p><ul><li>The price of the equity may exhibit nonlinear behavior, such as a fat tail distribution. This could lead to large losses for the lender if the price of the equity declines sharply.</li></ul></p><p><ul><li>Option and derivative positions leading to non-linear payoffs.</li></ul></p>|
|**4\. Bond**|<p><ul><li>The borrower may take on too much leverage, which could lead to a default</li></ul></p><p><ul><li>Use of bond futures for leverage.</li></ul></p>|<p><ul><li>The price of the bond may exhibit nonlinear behavior, such as a fat tail distribution.</li></ul></p><p><ul><li>Non-linear yield changes due to convexity (here, convexity is the derivative of the price of the bond with respect to interest rates.).</li></ul></p>|


**2: Frictional Related Challenges**

|**Scenario**|**Liquidity Challenges**|**Regulation Challenges**|
| :- | :- | :- |
|**1\. Unsecured Loan**|<p>- For a buyer, an unsecured loan is difficult to obtain if one doesn’t have a good credit score or enough assets. And interest rates are too high.</p><p>- From the bank's perspective, there is no collateral, so the loan will be fully recovered if default is not guaranteed. The selling of this asset class to third party becomes difficult</p>|<p>- Seeking higher interest rate banks not doing due diligence like credit assessment, default risk. So regulation is in place to maintain reserve ratios like CRR and SLR to meet its other obligations and have a proper risk management department.</p><p>- The borrower is not taking excessive debt when he has prior debt. Basel III Capital Framework, Fair lending regulations are there</p>|
|**2\.Construction Loan**|<p>- For a buyer, a loan is dependent on a good credit score or enough assets. And interest rates are too high if one has no collateral and/or high debt..</p><p>- From the bank's perspective, if there is no collateral, then it's the same as an unsecured loan. But if collateral is there, then construction may be incomplete or fall in prices of properties as collateral. So, recovery is less in defaulted loans.</p>|<p>- Same as above from the bank's perspective.</p><p>- For the business to not take excessive risk, there are regulations preventing him from borrowing much compared to his assets using debt-asset ratio and debt to equity ratio. Also businesses are required to be audited to be transparent to lenders and investors.</p>|
|**3\. Equity**|<p>- The market for equity lending may be illiquid, making it difficult to borrow the shares on margin.</p><p>- Market impact costs of large trades</p><p>- Limited availability of borrowable stocks</p>|<p>- There are regulations in place that govern the equity lending market. These regulations are designed to protect investors and to prevent market abuse:</p><p>1. Insider trading regulations</p><p>2. Market manipulation and fraud prevention</p><p>3. Short selling restrictions and regulations</p>|
|**4\. Bond**|<p>- The market for bond lending may be illiquid, making it difficult to borrow the bonds due to low trading volume.</p><p>- Limited availability of specific bond issues</p><p>- Difficulty in finding willing bond lenders</p>|<p>- There are regulations in place that govern the bond lending market:</p><p>1. Credit rating agency regulations</p><p>2. Securities lending regulations</p><p>3. Market transparency regulations</p>|

**3: Identifying Additional Data**

In addition to the data that was identified in Project 1, the following additional data could be collected to help address the magnifying risks and frictional challenges:

||**Unsecured Loan** |**Construction Loan**|**Stock**|**Bond**|
| :- | :- | :- | :- | :- |
|**Data Type**|Credit Rating, Accounting, Economic, Financial Aid|Credit Rating, Accounting, Market Outlook|Asset, Accounting, Market Data|Asset, Accounting, Market Data|
|**Data Processing** |Fico Scores, Family Income, Employment Outlook, Debts and assets.|Balance sheet, leverage ratios, solvency ratios, LTV, DTI|Returns, Volatilities, balance sheet ratios|Yields, Interest Rate, Inflation, balance sheet ratios |
|**Data Frequency**|Quarterly, Yearly    |Quarterly, Yearly|Daily |Daily, Quarterly, Yearly|
|**Data Class**|Credit, Social, Financial Statements|Credit, Real Estate, Financial Statements|Equity, Financial Statements|Fixed Income, Financial Statements |
|**Data Source** |CFPB, FRED, FRBNY|FRED, Yahoo Finance |Yahoo Finance |Yahoo Finance |
|**Data Variety**|Observed Data |Observed Data, Trade data, Actual data |Trade Data, Actual Data |Trade Data, Actual Data |

- Leverage: The amount of leverage that the borrower is taking on. This information can be obtained from the borrower's financial statements.
- Non-Linearities: The price behavior of the asset. This information can be obtained from historical price data.
- Liquidity: The liquidity of the market for the asset. This information can be obtained from the bid-ask spread and the volume of trading.
- Regulation: The regulations that govern the market for the asset. This information can be obtained from government websites and regulatory bodies.

**4: Describe how the data can help to meet the challenge**
**\
The data gathered last time helps address volatility and liquidity challenges:

- The equity and bond prices help evaluate the value and volatility of the collateral, aiding in determining **loan-to-value (LTV) ratios** and exposure to **market movements**.
- Volatility data assists in estimating risks and returns, enabling the team to make informed decisions on **lending rates** and **terms**.
- Correlation data provides insights into the interdependencies among securities, helping with **diversification strategies** and **risk management**.

The data gathered this time can be used to help address the challenges of magnifying risks and frictional challenges. For example, the data:

- Can be used to calculate **Key metrics** such as leverage ratios and the assessment of non-linear payoffs. 
- On **Leverage** can be used to assess the risk of a borrower defaulting and the amplification of losses and gains.
- **Nonlinearities** can be used to assess the risk of large losses and to come up with potential mitigation strategies.
- **Liquidity** can be used to assess the difficulty of borrowing an asset.
- On **Regulation** can be used to assess the compliance risks and hence steps to ensure adherence to the same.


**In summary, by collecting and analyzing this data, the financing team can make better decisions about lending money to borrowers, assess the risks involved and take steps to mitigate those risks. This will help to protect the team from losses and to ensure that the team is meeting its lending goals.**




**References**

1. “Jones Lang Lasalle Inc (JLL) Stock Price, Trades & News.” GuruFocus, [www.gurufocus.com/stock/JLL/summary](http://www.gurufocus.com/stock/JLL/summary). Accessed 10 July 2023. 
1. Folger, Jean. “What Is Considered a High Debt-to-Equity (D/E) Ratio?” *Investopedia*, 5 Apr. 2023, [www.investopedia.com/ask/answers/063014/what-considered-high-debttoequity-ratio-and-what-does-it-say-about-company.asp](http://www.investopedia.com/ask/answers/063014/what-considered-high-debttoequity-ratio-and-what-does-it-say-about-company.asp). 
1. Lee, Donghoon. *Household Debt and Credit: Student Debt*, Federal Reserve Bank of New York, 28 Feb. 2013, [www.newyorkfed.org/medialibrary/media/newsevents/mediaadvisory/2013/Lee022813.pdf?mod=article_inline](http://www.newyorkfed.org/medialibrary/media/newsevents/mediaadvisory/2013/Lee022813.pdf?mod=article_inline). 
1. DiNapol, Thomasi  P. *Student Loan Debt in New York State, September 2016*, Sept. 2016, [www.osc.state.ny.us/files/reports/special-topics/pdf/education-loan-debt-2016.pd](http://www.osc.state.ny.us/files/reports/special-topics/pdf/education-loan-debt-2016.pdf)[f](http://www.osc.state.ny.us/files/reports/special-topics/pdf/education-loan-debt-2016.pdf)
1. *Leverage Ratios - Meaning, Types, Calculation, Examples - Wallstreetmojo*, [www.wallstreetmojo.com/leverage-ratios/](http://www.wallstreetmojo.com/leverage-ratios/). Accessed 11 July 2023.
1. Srivastav, Ashish  Kumar. *Solvency Ratios (Formula, Example, List) - Wallstreetmojo*, [www.wallstreetmojo.com/solvency-ratios/](http://www.wallstreetmojo.com/solvency-ratios/). Accessed 11 July 2023. 

<a name="_3njj2xp27vi6"></a>
