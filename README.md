# Data-Extraction-using-Yfinance-and-Webscraping
Tesla and GameStop Case Study
This code is part of a case study that explores historical stock price and revenue data for two companies: Tesla and GameStop. The purpose of this code is to fetch historical stock price and revenue data, process and clean the data, and then visualize it using Plotly.

Prerequisites
Before running this code, make sure you have the following packages installed:

yfinance==0.1.67

bs4==4.10.0

nbformat==4.2.0

html5lib==1.1

lxml==4.6.4

You can install these packages using pip or mamba with the provided commands at the beginning of the code.

Code Description
The code begins by importing necessary Python libraries, including yfinance for fetching stock price data, BeautifulSoup for web scraping, and Plotly for data visualization.

The code fetches historical stock price data for Tesla using the Yahoo Finance API and stores it in a Pandas DataFrame.

Web scraping is performed to retrieve historical revenue data for Tesla from a specific URL. The HTML content is obtained using the requests library, and BeautifulSoup is used to parse the HTML data.

The revenue data is processed and cleaned. Any commas or dollar signs in the revenue values are removed, and empty or NaN rows are dropped from the DataFrame.

The make_graph function is defined to create a Plotly figure with two subplots: one for historical share prices and another for historical revenue. The data is filtered to include only data points up to specific dates (June 14, 2021, for stock prices and April 30, 2021, for revenue). The subplots are then created with appropriate labels and titles.

The historical stock price data and revenue data are passed to the make_graph function to generate a visualization that shows the historical share price and revenue trends for Tesla.

GameStop Case Study
To adapt this code for a GameStop case study, you can follow a similar process with the GameStop stock symbol ("GME") and revenue data specific to GameStop. Replace "TSLA" with "GME" when fetching stock price data and adjust the URL and data cleaning steps for GameStop's revenue data accordingly. The rest of the code, including data visualization, can remain unchanged.

This code serves as a valuable tool for analyzing and visualizing historical financial data for both Tesla and GameStop, making it easier to draw insights and conduct comparative studies between these two companies.
