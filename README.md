Project Overview:

The primary objective of this project is to develop predictive models for housing prices.

Notebooks:

EDA before Data Cleaning:
This notebook performs an exploratory data analysis (EDA) on the raw data, providing an initial understanding of the dataset.

Basic Data Cleaning Before Filtering:
In this notebook, data cleaning operations are performed, including the identification and handling of rows with incorrect information. Additionally, a comprehensive address column is generated using regular expressions. The resulting cleaned dataset is saved as "correct_real_estate.csv."

Data Cleaning to Filter by Remarks:
This notebook focuses on refining the dataset further. It ensures that data types are correctly labeled and filters the dataset based on the presence of remarks and location criteria. The cleaned dataset with remarks is saved as "real_estate_with_remarks.csv."

Geocoding Coordinates of Rows with Remarks:
In this notebook, geographical coordinates are obtained using the Open Street Map API for rows containing remarks. The process is based on the 'full address' field. The resulting dataset with updated latitude and longitude information is saved as "lat_lon_updated_for_real_estate_with_remarks.csv."

Data Cleaning After Geocoding:
This notebook focuses on the final stages of data cleaning. It involves the removal of redundant columns and the elimination of rows with missing values in the coordinate columns.
Raw Data Source:
Real Estate Sales 2001-2020 - CT.gov

Additional Files:

Presentation Slides

Tableau Visualization