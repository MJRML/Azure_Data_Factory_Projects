# Project: Real-Time Crypto Data Pipleline with Azure Data Factory and CoinGecko API

## Project Overview:

This project demonstrates how to build an end-to-end ETL pipeline using Azure Data Factory (ADF) to extract live cryptocurrency market data from the CoinGecko REST API, transform the JSON response, and store the results in an Azure SQL Database. Configure an automated trigger in Azure Data Factory to extract data from the CoinGecko API on an hourly schedule and update the records in the Azure SQL Database

### Project Goal: Fetch live crypto market data (top 100 coins by market cap) from CoinGecko API and transform the json file and store it in Azure SQL DB  

## Step 1: Create CoinGeko Account and request AKI Key

- Create an account and login to the CoinGeko  https://www.coingecko.com/
- Go to 'View Developer Dashboard' and create a new API Key (**Note One API Key allowed per Demo account**) (insert image 1)
- Here is the documnetation for creating an API Key https://support.coingecko.com/hc/en-us/articles/21880397454233-User-Guide-How-to-sign-up-for-CoinGecko-Demo-API-and-generate-an-API-key (insert image 2)
- The Root Url is mentioned in the documentation 


## Step2: Create Azure SQl Database and configure the Database table using Azure Data Studio

- Create the Azure SQL Database in the Azure Portal
- Once our Database is created select 'Open in Azure Data Studio' (Insert image 3)
- Connect to your database use your SQL credentials and create out table which will hold our CoinGeko Rest API data (insert image 4)


## Step 3: Configure Azure Data Factory to ingest the Data from CoinGeko and store it in our Azure SQL Database
