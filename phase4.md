# CSI4142-Project

### Mershab Issadien 300027272
### Alessandro Miguel Tirado 8349209
### Arthur Trakulkajornsak 300192223 

## Part A

1. Our data summarization visualizations exists on the BI Dashboard: 
[Click Here!](http://csi4142-metabase.mershab.xyz/public/dashboard/8276e647-29fd-4238-81dc-f04ca0f4f2d5)

2. When constructing the fact table we were forced to select only the tickers which exist in both the CEO_dimension and company_dimension. In addition, I had to average the stock closing price over the year as our cost_of_living_dimension data was stored by year. Cleaning the data to remove duplicate 'year_x' and 'year_y' columns as a result of the dataframe merging (effectively SQL joins). As regular SQL joins did not work (yielding no rows for obviously matching joins on ticker), we were forced to utilize pandas and construct the fact table using python dataframes. After merging the dataframes, we removed all the columns which belonged to the dimensions, copying the columns that are desired into snake case formatting, and then deleting the originals. What we are left with in the end is a clean fact table which contains cost of living by state, tied to each ticker, the average stock price for the year, and the CEO compensation for the same year. Along with a computed pay ratio between the CEO and median salary.

## Deliverables Part B

[Github Project Link!](https://github.com/Mershab99/CSI4142-Project)
