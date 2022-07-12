## Retrieving data from Google BigQuery
`SELECT value FROM `bigquery-public-data.crypto_ethereum.transactions` WHERE DATE(block_timestamp) BETWEEN "2020-01-01" AND "2022-07-06" LIMIT 1000`

### About how to use Etherscan API with Python, please see [Getcontracts.py](https://github.com/KerwinFuyihang/SmartBugs/tree/main/Code)

