<div align="center">
  <h3 align="center">Interactive Stock Sentiment Heatmap for Dow Jones Stocks</h3>
  <p align="center">
    Updated regularly using a customized workflow on GitHub Actions, with sentiments extracted from the newest headlines!
    <br />
    <a href="https://rajarshi1902.github.io/dow_jones_live_sentiment.html"><strong>Check it out here</strong></a>
  </p>
</div>

<!-- INSPIRATION -->
### Inspiration

This project is inspired from the treemap plots available on websites like FinViz, FinScreener and TradingView. That’s because treemap plots give such a good overall view of the market. The companies, in the example below, are from the S&P 500 index, the size of each box represents the market cap of each company relative to the whole index, while the numbers and colors represent the percentage change of the stock’s price.

<a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://miro.medium.com/max/1400/1*UGVVz1mQdJAzBzct7Rg5EA.png" alt="Check FinViz treemap" width="300" height="100">
  </a>
  
<!-- ABOUT THE PROJECT -->
### About the project
  
In this project, the Dow Jones tinkers are being analysed through their market decisions and the sentiment generated from it. The project is end-to-end starting from the scraper to the sentiment analyzer then finally the treeplot and hosting. 

The project has three parts: 
1. News Scraper : The scraper uses the FinViz website and extracts all news headlines for a particular tinker using Beautiful Soup. The data is then stored into a list which is then stored into a dataframe. You can checkout Sentiment_scraper.ipynb for details.
2. The dataframe is then fed into the Vader library which analyses each headline and allots it a score based on the analysis.
3. The dataset, along with the sentiments and other data required, is visualised in the treemap which is live. 


### Automation Setup

This project is set to be automated A workflow is configured in GitHub actions to install necessary libraries from requirements.txt, run the Python script "update_sentiment_page.py" that scrapes FinViz for financial headlines, perform sentiment analysis and generate the updated html page.

The html page is then pushed to my Github pages repository.

An accompanying Jupyter notebook "Heatmap_updated.ipynb" is included for exploration, it has similar code to the .py script and shows the output at every step.


<!-- USAGE EXAMPLES -->
### Usage

This treemap can be used to assist individuals to make financial decisions. That said, this project, by no means, is to be used solely for making investing choices. Please do your own proper research. 
