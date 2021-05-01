# LSTM-trader

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

High Level Overview:
1. Selected stocks from different industries/sectors
2. Cleaned the data by removing any NaN values and aligning the dates of the monthly data, and adding the stock header
3. Added technical features to the intraday data
4. Found which technical indicators have a high correlation with the
stock price and remove the rest
5. Trained the LSTM model with the selected features and predict prices
6. If the predicted price in i+holding_period length of time is higher
than the actual value of the stock price at time i, go long then short at time t= i+holding_period. If the predicted price is lower, reverse the strategy.
(The second iteration of this required the predicted stock price of the next time t= i+holding_period to be greater by the transaction fees and to be at least 20% above the current price)
7. Every transaction needed to be subtracted by 2.75 bsp
8. Calculated returns

### Built With

* []()Python


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these steps.

### Prerequisites

This is a list of packages that need to be installed before the notebook can be run.
* sklearn
* quandl
* BlockChair
* yFinance
* pandas
* numpy
* seaborn
* matplotlib
* scipy


### Installation

Clone the repo: https://github.com/calvinma888/Blockchain_Forex_Arbitrage.git
   

<!-- USAGE EXAMPLES -->
## Usage

Run with Jupyter Notebook


<!-- CONTRIBUTING -->
## Contributing

Calvin (Yu chien) Ma

