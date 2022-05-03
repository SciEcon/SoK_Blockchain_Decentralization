# Supplementary resources, data, and code for the research article:

**"The Decentralization Index of Blockchain Transactions: the Entropy of Token Transfers on Ethereum"** 

by *Yulin Liu, Xinshi Ma, and Luyao Zhang**

*names by alphabetical order, \*corresponding author*

## Data Files

**Decentralization Index of Top DeFi Tokens**
 |   **Name**   | **Token** | **First Observation Date** |  **File Name** |
 |:------------:|:---------:|:--------------------------:|:--------------:|
 |     Aave     |    AAVE   |         2020-10-02         |  Aave_ent.csv  |
 |   Compound   |    COMP   |         2020-06-14         |  Comp_ent.csv  |
 |     Maker    |    MKR    |         2017-12-15         |  Maker_ent.csv |
 |      Dai     |    DAI    |         2019-11-18         |   Dai_ent.csv  |
 |      Sai     |    SAI    |         2017-12-18         |   Sai_ent.csv  |
 |    Liquity   |    LQTY   |         2021-04-05         |  Lqty_ent.csv  |
 |    Uniswap   |    UNI    |         2020-09-18         |   Uni_ent.csv  |
 |   Sushiswap  |   SUSHI   |         2020-08-26         |  Sushi_ent.csv |
 |   Balancer   |    BAL    |         2020-06-20         |   Bal_ent.csv  |
 |    Bancor    |    BNT    |         2017-06-17         |   Bnt_ent.csv  |
 | Convex Curve |   CVXCRV  |         2021-05-17         | CVXCRV_ent.csv |
 |    Convex    |    CVX    |         2021-05-17         |   CVX_ent.csv  |
 | Fei Protocol |   TRIBE   |          2020-3-28         |  Tribe_ent.csv |
 |     RenVM    |    REN    |         2017-12-31         |   Ren_ent.csv  |
 |     Flexa    |    AMP    |         2019-01-09         |   Fxc_ent.csv  |
 | Tornado Cash |    TORN   |         2020-12-18         |  Torn_ent.csv  |
 |   Synthetix  |    SNX    |         2020-05-11         |   Snx_ent.csv  |
 | Nexus Mutual |    NXM    |         2019-05-23         |   Nxm_ent.csv  |

**Coinmetrics Market Data**
|   **Name**   | **Token** | **File Name** |
|:------------:|:---------:|:-------------:|
|    Bitcoin   |    BTC    |    btc.csv    |
|   Ethereum   |    ETH    |    eth.csv    |
|      Dai     |    DAI    |    dai.csv    |
|      Sai     |    SAI    |    sai.csv    |
|     Aave     |    AAVE   |  aave_met.csv |
|   Compound   |    COMP   |  comp_met.csv |
|     Maker    |    MKR    |  mkr_met.csv  |
|    Uniswap   |    UNI    |  uni_met.csv  |
|   Sushiswap  |   SUSHI   | sushi_met.csv |
|   Balancer   |    BAL    |  bal_met.csv  |
|     RenVM    |    REN    |  ren_met.csv  |
|   Synthetix  |    SNX    |  snx_met.csv  |
| Nexus Mutual |    NXM    |  nxm_met.csv  |

## Data Dictionary
**Coinmetrics Variables**
| **Variable Name** | **Unit**           | **Frequency** | **Description**                                                                                                                     |
|-------------------|--------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------|
| CapMrktCurUSD     | USD                | Daily         | Market capitalization in USD: The sum USD value of the current supply.                                                              |
| PriceUSD          | USD                | Daily         | The fixed closing price of the asset as of 00:00 UTC the following day                                                              |
| VtyDayRet30d      | Percent per annum  | Daily         | The 30 day volatility, measured as the standard deviation of the natural log of daily returns over the past 30 days.                |
| TxTfrValAdjUSD    | USD                | Daily         | The USD value of the sum of native units transferred between distinct addresses that interval removing noise and certain artifacts. |
| TxTfrCnt          | Number             | Daily         | Daily transaction count                                                                                                             |
Note: Description of other variables can be found in the [Coinmetrics Docs]( https://docs.coinmetrics.io)
