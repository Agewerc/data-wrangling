# Data Cleansing
![Imgur](https://i.imgur.com/EkkYyj0.png)

## Description
`data-cleansing.ipynb`:

This project focus on the analysis to find and fix the problems in a dataset containing restaurant orders. We perform graphical and non-graphical EDA methods to understand the data first and then find the data problems. The required tasks are the following:

1.  Detect and fix error in the dirty data: The dataset `dirty_data` contains in most of its columns wrong values that must be identified and replaced. 

2. Data Imputation: The dataset `missing_data` contains a relevant number of missing values in some of its columns. They will identified and imputation will me made by the most accurate possible method.

3. Detect and remove outliers: The dataset `outlier_data` contains a relevant number of outliers w.r.t. `delivery_fee` attribute, which would bias any regression or model used to fit it. They will be removed from the dataset.

It was developed using `python3` on Jupyter Notebook.

## Data
The dataset contains Food Delivery data from a restaurant in Melbourne, Australia. The restaurant has three branches around CBD area. All three branches share the same menu but they have different management so they operate differently. Each instance of the data represents a single order from said restaurant. There are a total of 1500 menu orders in three files of 210 KB. The following `CSV` files are originated from a single dataset and breaked in a didactic way:

* `dirty_data.csv`: 

   Contains syntactic, semantic, and coverage anomalies to be found and handled.
* `missing_data.csv`: 

   Contains missing data to be imputed.
* `outlier_data.csv`: 

   Contains outliers to be found and handled.
   
   There are also three support files, of total 2.2 MB.:
* `branches.csv` 

* `edges.csv`

* `nodes.csv`

## Output
The data is cleaned using the proper treatments in order to generate the output.

* `dirty_data_solution.csv`
   
* `missing_data_solution.csv`

* `outlier_data_solution.csv`