# Data Cleansing
![Imgur](https://i.imgur.com/EkkYyj0.png)

## Description
`data-cleansing.ipynb`:

This project focus on the analysis to find and fix the problems in a dataset containing restaurant orders. Problems studied:
1. Syntactic, semantic, and coverage anomalies.
2. Missing data.
3. Outliers.

It was developed using `python3` on Jupyter Notebook.

## Data
The dataset contains Food Delivery data from a restaurant in Melbourne, Australia. The restaurant has three branches around CBD area. All three branches share the same menu but they have different management so they operate differently. Each instance of the data represents a single order from said restaurant. The following `CSV` files are originated from a single dataset and breaked in a didactic way:

* `dirty_data.csv`: 

   Contains syntactic, semantic, and coverage anomalies to be found and handled.
* `missing_data.csv`: 

   Contains missing data to be imputed.
* `outlier_data.csv`: 

   Contains outliers to be found and handled.
## Output
The data is cleaned using the proper treatments in order to generate the output.

* `dirty_data_solution.csv`
   
* `missing_data_solution.csv`

* `outlier_data_solution.csv`