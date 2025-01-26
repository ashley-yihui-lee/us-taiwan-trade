This repository contains code for an automated monthly scraper of Taiwan-US trade data since January 2023.

Trade data is sourced from the Import and Export Statistics of Taiwan’s International Trade Administration (https://www.trade.gov.tw/Pages/Detail.aspx?nodeID=1375&pid=790878&dl_DateRange=all&txt_SD=&txt_ED=&txt_Keyword=&pageindex=1&history=).

- **taiwan-us-trade.ipynb**: Scrapes and cleans data from the Taiwan ITA Excel file.
- **11310-我國對美國出進口統計總表.xls**: Raw Excel file from the Taiwan ITA website.
- **taiwan-us-trade.csv**: Cleaned dataframe.
- **data diary.ipynb**: Notes on the coding process.
- **index.html**: Code for the live website [US-Taiwan Trade](https://ashley-yihui-lee.github.io/us-taiwan-trade/), displaying an auto-updating line chart of Taiwan-US trade.

-

Here are the things I did in this project
1. Scraping
Scrapes the Taiwan’s International Trade Administration website for the latest Taiwan-U.S. trade data.
Identifies and downloads the relevant Excel file.

2. Cleaning the Data
Removes unnecessary rows and columns from the dataset.
Handles missing or improperly formatted data.
Converts Taiwanese year format (ROC) to the Gregorian calendar.
Maps month names to standard English abbreviations.
Filters and organizes the data for the year 2023 onward.

3. Export to CSV
Outputs the cleaned and processed dataset as taiwan-us-trade.csv.

4. Auto-Update
Automates the data scraping and processing workflow using GitHub Actions.
