**Project Overview**

The primary objective of this project is to develop predictive models for housing prices.

The raw data file was obtained from https://catalog.data.gov/dataset/real-estate-sales-2001-2018.

**Data Dictionary**

`serial number`: Serial Number

`list year`: Year the property was listed for sale

`date recorded`: Date the sale was recorded locally

`town`: Town name

`address`: Address

`assessed value`: Value of the psroperty used for local tax assesment

>With the exception of certain classified land, the assessment of each parcel of real property represents 70% of its estimated fair market value as of the date of a revaluation (Chapter 203 - Sec. 12-62, Sec. 12-62a and Sec. 12-63)

`sale amount`: Amount the property was sold for

`sales ratio`: Ratio of the sale price to the assessed value

`property type`: Type of property including: Residential, Commercial, Industrial, Apartments, Vacant, etc

`residential type`: Indicates whether property is single or multifamily residential

`Non Use Code`: Non usable sale code typically means the sale price is not reliable for use in the determination of a property value. See attachments in the dataset description page for a listing of codes

`Assessor Remarks`: Remarks from the  municipal assessor

`OPM remarks`: Remarks from OPM, Office of Policy and Management

`Location`: Lat / lon coordinates


**Notebooks**

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

**Additional Files**

Presentation Slides

Tableau Visualization