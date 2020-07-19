# Data Integration and Reshaping
![Imgur](https://i.imgur.com/Gaq0kNy.png)

## Description
`data-integration-reshaping.ipynb`:

`Python3` code to integrate several datasets into one single schema and find and fix possible problems in the data. The final dataset integrates multiple sources aiming to generate an extensive source for housing analysis in Melbourne, Victoria.

* Integrates `XLSX` crime data, `TXT` council data, `XML` school location data, `web scraped` school rakings, `SHP` Victoria boundary data, `PTV GTFS` transportation data and `CSV` real estate data. 

* Studies the effect of different normalization/transformation methods (i.e. standardization, min-max normalization, log, power, and root transformation) on some  attributes.

## Data
There is information about schools, crime, properties details and public transportation.

* the vic_suburb_boundary data `VIC_LOCALITY_POLYGON_shp.*` containing the shapefile data about Victoria's suburbs. This data is needed to calculate the suburb attribute of the final dataset. 
* the gtfs dataset. This data is essential to retrieve information about the transport system. This data was too large to include here, but can be downloaded at [PTV GTFS](https://transitfeeds.com/p/ptv/497). You can download the most recent version, but probably will get slightly different results. The one we used was from October 2019. Please include the unzipped folders in **data** and refer to the documentation in the Jupyter Notebook to a better understanding.
* the crime statistics dataset `crimebylocation.xlsx`. This data is used to retrieve crime attributes.
* the council dataset `councils.txt`. This data can be used to map the suburb to a local government.
* the schools dataset `schools.xml`. Data to retrieve school information. 
* the school ranking information was scraped from [Primary Schools](http://www.schoolcatchment.com.au/?p=12301). Due to permission issues, the secondary data was made available here in `secondary_rank.xml`. 
* the real state dataset `real-estate.csv`. Data to retrieve information about the properties.

For further details, refer to `data-integration-reshaping.ipynb`.

## Output
The data is integrated and reshaped in order to generate the output, which includes extensive information on 678 properties. All 26 features are detailed on the `.ipynb` file.

* `solution.csv`
