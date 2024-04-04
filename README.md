# COVID-19 Data Analysis and Forecasting

This repository contains Python code for analyzing COVID-19 data and forecasting active cases and recovery cases using the Prophet library. The data used in this analysis covers the period from January 22, 2020, to June 18, 2020.

## Requirements

To run the code in this repository, you need the following libraries installed:

- pandas
- matplotlib
- seaborn
- plotly
- prophet

You can install these libraries using pip:

```bash
pip install pandas matplotlib seaborn plotly prophet

Data Source
The COVID-19 data used in this analysis is sourced from the following CSV file:
'https://raw.githubusercontent.com/dsarosh/Sarosh-Dastoor/main/covid_19_clean_complete_till_23_June.csv'

Analysis and Forecasting Steps
Data Preprocessing

Loading the COVID-19 data into a pandas DataFrame.
Converting the 'Date' column to datetime format.
Dropping unnecessary columns ('Province/State').
Renaming columns ('Country/Region' to 'country').
Calculating the number of active cases and adding it as a new column ('Active').
Data Visualization

Plotting active cases on a world map using Plotly Express.
Plotting confirmed cases vs. date using seaborn point plots.
Comparing confirmed and death cases using seaborn point plots and scatter plots.
Top Countries Analysis

Identifying and plotting the top 20 countries with the highest active cases.
Country-Specific Dataframes

Creating separate DataFrames for China, India, Italy, US, and Germany.
Analyzing and plotting recovery rates for these countries.
Forecasting Using Prophet

Forecasting confirmed, death, active, and recovery cases for India using Prophet.
Generating forecasts for a specified period and plotting the forecasts.

