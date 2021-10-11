# Project Title

This is the Financial Planner Application for challenge 5! The first part of the applications pulls in current pricing data
for Bitcoin and Ethereum. I have a theoretical holding of each coin, and I calculate the individual as well as combined
holding values of my crypto currency position.

For the second part of the application I pull in the most recent closing price (2021-10-08 at the time of this writing) for an equity and bond fund.  I use an Alpaca SDK call to do that. I then assume I have 110 shares of the equity fund and 200 for the bond fund.
I calculate the value of my equity and bond portfolio holdings, and then sum this value to my crypto currency holding value from the first part. After I calculate the individual pieces of the total portfolio I plot a pie chart showing the breakdown of the holdings.

I now multiply my monthly income by 3 and call that my emergency fund. I compare it to the value of my current holdings. If my holdings are greater than or equal to my emergency fund, I am happy. If my emergency fund goals are greater than my current holdings, I take a difference and let the user know how many dollars short I am from being able to fully fund my emergency fund.

The next step in the application is assume a 40% / 60% weighting between the bond and equity holdings and run a monte carlo
simulation for 30 years and calculate the 95% confidence interval of where the monthly income of 12000 could possibly take us.

 I run the same analysis as above but for 10 years and assuming a 20% / 80% weighting in favor of equity holdings.


## Story

You’ll create two financial analysis tools by using a single Jupyter notebook:

A financial planner for emergencies. The members will be able to use this tool to visualize their current savings. The members can then determine if they have enough reserves for an emergency fund.

A financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

You’ll use the information from the Monte Carlo simulation to answer questions about the portfolio in your Jupyter notebook.


---

## Technologies

I am using python version 3.7.10 and am importing the following from the built-in libraries and from functions i've created myself:
import pandas as pd
from pathlib import Path
%matplotlib inline

---

## Installation Guide

I have python version 3.7.10 and git version 2.33.0.windows.2 installed on a laptop running windows 10 pro.

I launch jupyter lab from the gitbash terminal and then run the risk_return_analysis noteback from the 
webpage that launches.


---

## Usage

I have one csv file in the Resources folder named whale_navs.csv.  All that needs to be
done by the user is hit the double arrow and run the code. 

That's it!


---

## Contributors
Just me, Paul Lopez.


---

## License
No licenses required. Just install everything for free, pull from my repository, and enjoy!
