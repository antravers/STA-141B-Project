# STA 141B Project Proposal
## Group 6
#### Aurora Travers  -  antravers@ucdavis.edu 
#### Ivan Louize Winoto - ilwinoto@ucdavis.edu 
#### Alex Prado - alxprado@ucdavis.edu 
#### Lilly Patty - lpatty@ucdavis.edu 
#### Young Ha - yhajeong@ucdavis.edu

The topic of our project is preserving recommended nutritional intakes while finding the most optimal cost saving. We will attempt to determine which food combinations provide the required nutritional values with the lowest price by implementing using the simplex algorithm. The question that we want to answer the following: 

* Could we apply a methodology between the interactions of food, prices, and nutrition, to find an optimal minimal cost while maintaining nutritional requirements?

George Stigler won the Nobel Prize in Economics in 1982 for trying to answer this question using linear optimization techniques; the solution was named the Stigler Diet. Seven years later George Dantzig came up with the simplex algorithm, which generalized the solutions to a family of linear optimization problems. In this project, we aim to collect the data of food contents, nutritional values, pertaining price, and finally apply the simplex algorithm to find an optimal, Stigler Diet solution. While the Stigler diet is not recommended for its lack of food diversification, it could potentially be used to reduce food cost in specific cases. 

Current high inflationary food pricing makes the project meaningful, particularly for people of modest means who face food insecurity. Therefore, it is a priority to find food that contains recommended nutritional intakes and value for an optimal minimal price.

The data sets will have to come from two places. The first dataset will be the nutritional contents of common food types. The following provided links are places data can be generated from:

* https://www.nutritionix.com/database: Largest Free API Database for nutrition

* https://www.nutritionvalue.org/: Free API database tracker for nutritional value
 
* https://fdc.nal.usda.gov/: integrated data system that provides expanded nutrient profile data and links to related agricultural and experimental research.
 
The second data set will contain the respective food prices from multiples local food stores (i.e.; Trader joes, Walmart, etc) and from government institutions that track food prices:

* https://www.simplegrocerydeals.com/tag/prices/: Price list for walmart, trader joe, costco, etc -Jan 2023)

* https://www.traderjoes.com/home/products/category/food-8: Base data scraping Trader Joe’s source

* https://www.walmart.com/cp/food/976759: Base data scraping Walmart source. Although it might be hard. While Walmart has an API, a request to Walmart needs to be made to have access for any company interested in selling Walmart products (https://walmart.io/docs/opd/introduction)    

* https://www.ers.usda.gov/topics/food-markets-prices/food-prices-expenditures-and-establishments/: U.S. Department of agriculture online site to monitors indicators of individual, household, and market-level food consumption, prices, expenditures, food marketing costs, and farm-to-retail price spreads.

* https://comparegroceryprices.org/search/grocery-price-comparison.shtml: old additional data about food pricing

* https://www.ers.usda.gov/data-products/fruit-and-vegetable-prices/: data from 2018

* https://fred.stlouisfed.org/series/WPU01110205: an example of CPI of avocados

* https://www.bls.gov/regions/mid-atlantic/data/averageretailfoodandenergyprices_usandwest_table.htm: a generalized sample of food data

The data above in many ways is either incomplete or will have to be scrapped. While the CPI index data is available and helpful, we are interested in current food prices. The current food price can be calculated from the CPI if the base price is known, in which case elementary algebra can be applied to find the current price.

The project is challenging for three main reasons. First, the data collection must be accomplished through either direct download, APIs, and data scraping. This may be the most challenging part, as there aren’t good sources to find specific food prices. According to several librarians, it is mostly industry data used by private organizations to track it and sell it. The government either has outdated information on food prices, or no data at all. CPI data is available, and as previously said, the difficulty will be to find base prices in comparison with the base year of the cpi to find the current price.

Second, the data wrangling process needs to be done as well. Merging data from multiple sources, dealing with data gaps, or statistical outliers will have to be properly addressed. Eventually, food price data will have to be combined with their respective nutritional values.

Third, the actual application of the simplex algorithm. Thankfully there are several books and resources online about the implementation of the simplex algorithm. To complete this project we will rely heavily on the skills learned from STA 141B , such as web scraping. We will use Python, Jupyter Notebook or Google Colab. We will also use Matplotlib to show static visualization and use web APIs to gather the data we are going to use.
