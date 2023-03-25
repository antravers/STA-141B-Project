# Stigler Diet Project
Our full report can be viewed by the file FinalProject141.html

## Abstract
This paper aims to address the classic Stigler Diet problem by incorporating up-to-date supermarket data and nutritional information from the US Department of Agriculture. The study begins by scraping food prices and food names from dynamic supermarket websites by using Python libraries Selenium, and BeautifulSoup. To associate the scraped food items with their corresponding nutritional values, the Levenshtein distance is employed as a similarity measure between food names corresponding to nutritional values found in the US Department of Agriculture. The primal-dual path-following method, an interior-point algorithm for solving linear programming problems, is utilized to find the optimal Stigler Diet.
## Introduction
The Stigler Diet problem is a classic optimization problem in linear programming, proposed by George Stigler in 1945 for whcih he late rwon the Nobel Prize. The goal of the problem is to find the least expensive combination of foods that meets a given set of nutritional requirements. Stigler used data on food prices and nutritional content to identify a diet that would minimize the cost while satisfying the recommended daily allowances (RDAs) of various nutrients. However, it has the following limitations:
* Individual nutrient requirements can vary based on factors such as age, gender, activity level, and health status.
* It focuses solely on minimizing cost, disregarding factors such as taste, cultural preferences, and individual food aversions (like food allergies).
* It does not account for the importance of variety and a balanced diet.
* Food prices, availability, and nutritional content may change over time.
* It misses other essential nutrients or non-nutrient factors that contribute to a healthy diet.
