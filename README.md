# SmartBugs
This repo abstracts the data, results, and the commanding codes. Our research report on SmartBugs that how we can use this framework to analyze or evaluate the existing mainstream smart contract vulnerability detection tools and to retrieve SC vulnerability datasets. And we are sincerely imdebted to the amazing work by @jff @pedrocrvz who is the establisher of this framework.
For more detail about SmartBugs, please see [Github Page](https://github.com/smartbugs)

## Introduction of this repository
### Figure illustration of the SmartBugs Framework
<img width="1177" alt="Screen Shot 2022-07-04 at 14 06 49" src="https://user-images.githubusercontent.com/109135319/178464891-07c9eea4-1eea-4588-a87a-29bbebbddc16.png">

SmartBugs is consisted of system requirements, available tools and datasets, methodologies for adding tools and filtering datasets, and the available interfaces. The command-line interface, tool configurations, tool Docker images, datasets for smart contracts, and the SmartBugs Runner, which combines all of the components to run the analytic tools, are the five primary components of SmartBugs. SmartBugs is ditributed by 10 mainstream SC vulnerability detection tools and two existing datasets, SB curated & SB wild. 

In our research report, we introduced step-by-step guidline to access SmartBugs and use it to evaluate the performance of the detection tools. We retrieved the data from Google BigQuery. (if you want to see the detailed information of those two datasets above, please see [SB Curated](https://github.com/smartbugs/smartbugs) & [SB wild](https://github.com/smartbugs/smartbugs-wild)) We will introduce the data we retrieve and the step-by step guideline. The results, codes, and the data can be found respectively in the folders of this repository.

### Flowchart of our work
![4cec61cb-aaa2-4d63-87e6-7e780983fe01](https://user-images.githubusercontent.com/109135319/178493317-8c7bfb6a-4820-4258-86b2-dc9df99c2f55.png)

## Data Description 
### Features of Smart Contract vulnerability 
|Name|Description|
|----|-----------|
|Reentrancy|Reentrant function calls make a contract to behave in an unexpected way|
|Access Control|Failure to use function modifiers or use of tx.origin|
|Arithmetic|Integer over/underflows|
|Unchecked Low Level Calls|Unchecked Low Level Calls|call(), callcode(), delegatecall() or send() fails and it is not checked|
|Denial Of Service|The contract is overwhelmed with time-consuming computations|
|Bad Randomness|Malicious miner biases the outcome|
|Front Running|Two dependent transactions that invoke the same contract are included in one block|
|Time Manipulation|The timestamp of the block is manipulated by the miner|
|Short Addresses|EVM itself accepts incorrectly padded arguments|
|Unknown Unknowns|Vulnerabilities not identified in DASP 10|

### 



