## 1. [Coinmetrics Market Data](https://github.com/SciEcon/SoK_Blockchain_Decentralization/tree/main/Data_Coinmetrics)

### 1.1 Table of Data Files

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

### 1.2 Data Dictionary

| **Variable Name** | **Unit**           | **Frequency** | **Description**                                                                                                                     |
|-------------------|--------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------|
| CapMrktCurUSD     | USD                | Daily         | Market capitalization in USD: The sum USD value of the current supply.                                                              |
| PriceUSD          | USD                | Daily         | The fixed closing price of the asset as of 00:00 UTC the following day                                                              |
| VtyDayRet30d      | Percent per annum  | Daily         | The 30 day volatility, measured as the standard deviation of the natural log of daily returns over the past 30 days.                |
| TxTfrValAdjUSD    | USD                | Daily         | The USD value of the sum of native units transferred between distinct addresses that interval removing noise and certain artifacts. |
| TxTfrCnt          | Number             | Daily         | Daily transaction count |     

### 1.3 More about Data Source
Description of other variables can be found in the [Coinmetrics Docs]( https://docs.coinmetrics.io)
