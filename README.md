# Predicting the Non-Fungible

Estimated project completion date: April 23, 2022.

## Team:
- Harrison Hall
- Christina Li
- Andre Ray

University of Michigan, School of Information.
Master of Information, Big Data Analytics.
SI 699 - MSI Mastery Course.

**Project timeframe**: September 2021 - April 2022.


## Table of Contents:
- **README.md** - This lovely document, which you're reading now :)
- **model_data.csv** - Final dataset we use for modeling.
- **modeling/**
	- <i>data_compilation_LSTM.ipynb</i> - Notebook for merging the Trends and Twitter data, also for building and evaluating the initial LSTM.
	- <i>harrison-ml.ipynb</i> - Active notebook for testing different models.
- **data_collection/**
	- <i>collection_names_only.txt</i> - Initial list of names for relevant collections. Includes name & name + " NFT" for Trends (deprecated)
	- <i>collection_names_scraper.ipynb</i> - Script for grabbing the collection names from sales_records
	- <i>collection_names.txt</i>
	- <i>NFT_Daily_Transactions.csv</i> - For future development; data to possibly integrate with twitter+trends.
	- **opensea/**
		- <i>get-collections.ipynb</i> - Initial notebook for parsing user's wallets.
		- <i>initial-research.ipynb</i> - Testing which APIs we can freely access, exploring limitations.
		- **data/**
			- <i>initial_opensea_get_collections.csv</i> - output of initial-research.ipynb for testing
			- <i>opensea_get_many_collections.csv</i> - output of get-collections.ipynb, data scraped from wallets.
			- <i>opensea_traits.csv</i> - future reference only. Saved traits of each NFT; not used in this project.
	- **sales_records/**
		- <i>"... - Historical Sales.csv"</i> - All transactions we could scrape for each NFT, with prices.
		- **Andre_sales_records_1-50/**
			- Duplicates of "... - Historical Sales.csv" - Temporary fix for notebook efficiency.
		- **Andre_sales_records_100-150/**
			- Duplicates of "... - Historical Sales.csv" - Temporary fix for notebook efficiency.
		- <i>sales_data.csv</i> - Formatted transaction data for each NFT combined into 1 dataset.
	- **trends/**
		- <i>initial-trends-work.ipynb</i> - Initial testing of PyTrends wrapper, with function descriptions.
		- <i>trends-gathering.ipynb</i> - Final script for gathering trends data on all collections.
		- **data/**
			- <i>collection_names_plus_nft.txt</i> - Deprecated. List of collection names and collection_name + " NFT" for initial Trends searching
			- <i>daily_interest.csv</i> - Final output of trends-gathering.ipynb. The dataset we merge with Twitter.
			- <i>mint_dict.pkl</i> - Pickle file for sharing the dictionary of minting dates for each NFT.
			- <i>mint_json.json</i> - Same as mint_dict.pkl but as .json
			- <i>monthly_interest_over_time.csv</i> - Deprecated. Grabs Trends data weekly instead of daily.
			- **old/**
				- <i>trends_expanded_keywords.csv</i> - Output from (deprecated) initial-trends-work.ipynb, data on keyword expansion from PyTrends wrapper.
				- <i>trends_rising_queries.csv</i> - Output from (deprecated) initial-trends-work.ipynb, data on trending queries from PyTrends wrapper.
				- <i>trends_top_queries.csv</i> - Output from (deprecated) initial-trends-work.ipynb, data on top queries from PyTrends wrapper.
