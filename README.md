# SoK: Blockchain Decentralization
Read our paper on arXIV:[arxiv.org/abs/2205.04256](https://arxiv.org/abs/2205.04256)
## *Supplementary resources, data, and code*

[![DOI](https://zenodo.org/badge/461721882.svg)](https://zenodo.org/badge/latestdoi/461721882)

by **Luyao Zhang\*<sup>+</sup>, Xinshi Ma<sup>+</sup>, and Yulin Liu\*<sup>+</sup>**

\*: joint corresponding authors

<sup>+</sup>: joint first authors

![SoK: Blockchain Decentralization](https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/fig9.png)

|   **Folder**   | **Contents** | 
|:------------|:---------|
|   Data_Coinmetrics | ERC20 Tokens market metrics and data |   
|  Data_TokenIndex | Decentralization Index (Updated Daily) |  
|   Data_EIP1559 | EIP1559 adoption data |   
|  code | Code used to produce analysis in the paper  |  
|  tutorial | Sample calculation of Decentralization Index  |  
|conference_invitations| | 
|figures| | 


# Table of Contents

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

## 2. [Data_TokenIndex](https://github.com/SciEcon/SoK_Blockchain_Decentralization/tree/main/Data_TokenIndex)

### 2.1 Table of Data Files: Decentralization Index (Shannon Entropy) of Top DeFi Tokens

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
 
### 2.2 Data Dictionary: Decentralization Index of Top DeFi Tokens
 
 | **Variable Name** | **Unit** | **Frequency** | **Description**                                                                                              |
|-------------------|----------|---------------|--------------------------------------------------------------------------------------------------------------|
| val               | N/A      | Daily         | Decentralization Index value of transaction decentralization over the entire day before 00:00 UTC the following day |
| date              | N/A      | Daily         | The corresponding date index was calculated for    

### 2.3 More about Data Source: Decentralization Index of Top DeFi Tokens

Caculated from Google [BigQuery Ethereum dataset token](https://cloud.google.com/blog/products/data-analytics/ethereum-bigquery-public-dataset-smart-contract-analytics) transfers table. 

## 3. [Data_EIP1559](https://github.com/SciEcon/SoK_Blockchain_Decentralization/tree/main/Data_EIP1559)

### 3.1 Data Dictionary
| Variable Name     | Unit             | Frequency  | Description                                                                                           |
|-------------------|------------------|------------|-------------------------------------------------------------------------------------------------------|
| block_number      | None             | Per Block  | Unique identifier for each block in the blockchain. Used to reference and access specific blocks.     |
| all_gpcount       | Count            | Per Block  | Total count of transactions at different gas prices within a specific block or set of blocks.         |
| all_mfcount       | Count            | Per Block  | Total count of maximum fees associated with transactions in a block.                                  |
| all_prcount       | Count            | Per Block  | Count of transactions given a priority status, possibly due to higher fees or other criteria.         |
| legacy_gpcount    | Count            | Per Block  | Count of transactions using the old gas price system.                                                 |
| timestamp         | Unix Time        | Per Block  | Timestamp indicating when the block was mined, typically recorded in Unix time.                       |
| lag_timestamp     | Unix Time        | Per Block  | Timestamp of the previous block, used to calculate time intervals between consecutive blocks.         |
| block_time        | Seconds          | Per Block  | Duration between the current block and the previous block, measured in seconds.                       |

## 4. [Code](https://github.com/SciEcon/SoK_Blockchain_Decentralization/tree/main/code)

| **Content** |**Section of Paper**| **URL** |
|:---------|:--------------------------| :--------------------------| 
| Decentralization_Classes| Section 4: Data and Empirical Analysis  |https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/code/Decentralization_Classes.ipynb       |  
|   Top_DeFi_Decentralization_Visualizations | Section 4.2: Descriptive Analysis |https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/code/Top_DeFi_Decentralization_Visualizations.ipynb |  
|SAI_DAI_Decentralization_Analysis | Section 4.3: Predictive Analysis |https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/code/Top_DeFi_Decentralization_Visualizations.ipynb |
|Decentralization Index Daily Update| N/A | https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/code/daily-query.ipynb |
| EIP-1559 Analysis|  Section 4.4: Causal Inference |https://github.com/SciEcon/SoK_Blockchain_Decentralization/blob/main/code/EIP1559_Analysis.ipynb|




