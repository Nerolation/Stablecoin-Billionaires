# Stablecoin Billionairs
### Python Code of the Master Thesis by Anton Wahrstätter 

###### The code of this repo was continously improved and moved to [this space](https://github.com/Nerolation/ethereum-datafarm). Use it to collect your own data instead of the notebooks of this repo.


This is the official repository, which was created to descriptively analyze the Ethereum-based Stablecoin ecosystem in my [master thesis](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3737404). Alongside the paper, I publish the Python code used to examine Event data of specific Tokens.

Basically, the code is split into 5 separate python scripts, all created in Jupyter:


- ##### data_collection.ipynb
###### Used to fetch Event data from Ethereum via the [Etherscan API](https://etherscan.io/apis). Can be ecexuted one cell after another or  via the console. The script provides a flexible interface to collect data of a specific token and save it as csv files. As Etherscan's API comes with limits, the script automatically adjusts the requested blockrange in both direction to ensure that the process is as fast as possible without exceeding any limits. 
<br>

- ##### data_verification.ipynb
###### Script to verify the correctness of the data. This was done by collecting the same data from another source (via an Infura node) to then compare the data
<br>

- ##### data_processing.ipynb
######  In the data processing script, 'raw' events like Transfers, Mints and Burns were aggregated and further processed to create the final plot data. Note that this script requires huge amounts of RAM. During research I enjoyed working on a 24 GB RAM machine and especially Tether often foced me close to the borders.

<br>

- ##### data_analytics.ipynb
###### This script contains the code that assisted the main analytics part of the thesis. Again, much RAM is required to reproduce everthing. 
<br>

- ##### data_plotting.ipynb
###### Finally, the data plotting script was used to create the charts used in the paper.
<br>


<br>



##### Furthermore there are seven scripts incorporating the individual tokens analyzed. These are Tether USD, USD Coin, DAI Stablecoin, Paxos Standard, TrueUSD, HUSD and Binance USD. They include both, desprivtive statistics and the creation of charts.

<br>

##### Note that out of storage limitations on Github, this reposirtory doesn't contain the raw event data used for the analysis. Furthermore the files containing data about balances were to large to upload. [Click here](https://toniwahrstaetter.com/stablecoin_data.html) for the complete data set. 


Finally, due to time constraints, I did not optimize the analysis scripts to be fast and memory-efficient. The machine I was using had 24 GB of Ram, which was barely enough to handle the scripts in one execution. There is still much room for improvement, but unfortunately I am not able to do so at present.


<br>

#### Innsbruck, at 1. Oct 2020, [Anton Wahrstätter](https://toniwahrstaetter.com/)
