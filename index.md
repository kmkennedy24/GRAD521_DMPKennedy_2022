# Data description

My research is concerning steelhead salmon and the habitat they occupy in various Oregon watersheds. 
In my project I will be addressing questions regarding the relationship between different habitat characteristics, how changes in these habitat variables may impact steelhead populations, and how valuable some methods of data collection are compared to others in understanding these fish. 
I will be using existing datasets which have already been collected by others from Oregon Department of Fish and Wildlife. These data include:

- Surveys and describe various components of steelhead and coho salmon habitat along streams in Oregon as well as population data for each species. These data exist in multiple .csv files which I have been analyzing using R in R studio. 
- Spatial data which can be helpful in visualizing these habitat data while also layering in remotely sensed data about larger scale habitat data. These data are many different data types and are stored in a shared drive. They can be accessed and visualized by using ArcGIS, Python or R.
- Model outputs from a model called VELMA (Visualizing Ecosystem Land Management Assessments). These outputs include spatial layers related to hydrology and biochemistry. The outputs are ArcGIS layers and can be visualized by using ArcMap or other GIS platforms. 
- I hope to integrate Traditional Ecological Knowledge in my project to help inform my models. This may include interviews and transcriptions. 

All of these data will all be useful in developing species distribution models for juvenile steelhead salmon. Species distribution models use multiple covariates to project the presence or absence of individuals. I will mainly use these habitat data to decide the covariates and other components of the model. I have not assessed the most influential habitat characteristics in determining the likelihood of presence or absence, but will likely run a series of linear regression models to evaluate the importance of things like number/percent of pools identified, percent of down woody debris, and percent of shade. These models will likely be run in R, Python and ArcGIS. 
	
I have access to an abundance of data; however, it is unclear how much I will actually use in my project. Currently there is about 1-2 GB of datasets, however I expect as I develop multiple ArcGIS layers this number will increase to potentially 3-4 GB.  

# Roles and Responsibilities

My advisor (PI) would likely hold me accountable for implementing the DMP we organize together; however, 
I believe it would be my responsibility to implement the plan. My project is based on existing data and a dimension of my work will include acquiring, organizing, storing, and analyzing these data sets. 
Therefore, I will be solely responsible for these tasks as well as developing a system of archiving both the data and my analyses. Metadata is largely not included in the datasets I have acquired and because of this I have and will continue to contact the original owners of the data to generate metadata. Datasets from Oregon Department of Fish and Wildlife (ODFW) include raw fine scale habitat data for steelhead and coho salmon as well as population data. I may request data access to more habitat and population from NOAA. 
	
Since I will be using data collected by other people, 
I plan to make copies of all of these datasets and store the data in a separate folder of the Box drive that I share with my project partners. This will also be the location of my analyses generated in R. The owners of the Box drive are the PI as well as our partners at ODFW, therefore information will not be lost after I graduate. The Box drive will be the sole location for all data, however for data which is larger (i.e. VELMA model outputs) these will be exchanged through a hard drive which is the property of OSU. All datasets will be stored as .csv to ensure accessibility and all analyses will be accessible through RStudio, and open source platform. All spatial data layers will be stored together as zip files to ensure that all of the necessary data to view the layers is together. 
	
As my project continues I will develop models to analyze the population and habitat data. I hope to develop a package in R to store these methods of analysis as well as the metadata behind each step within the models. I will include all of this information as well as instructions of reproducibility within the package help files. 
	
To ensure that the changes I make to dataset format, as well as new data I develop through my various analyses, I plan to develop a file naming convention as well a visual guide for the DMP. This visual guide will display the location of files, the system of organization, as well as the contact information for those who are associated with the data who may be helpful resources. 

# Sharing, Archiving and Preservation

There are not any factors that limit the ability to share data with my project. However, there may be some datasets which do not communicate any information without access to GIS software. Besides for potential technological barriers, the information is unrestricted and will be shared publicly. Some of the data used in this project is already available upon request on the ODFW Data Clearinghouse website:
	
	https://nrimp.dfw.state.or.us/DataClearinghouse/default.aspx?ReturnUrl=%2fDataClearinghouse


Any products of my own research including GIS layers, mathematical models used for analysis, written reports, and other datasets will be publicly available in this same clearing house and the OSU data depository, ScholarsArchive@OSU:


	https://ir.library.oregonstate.edu/


While there are many sources of data in the ODFW Clearing House, the instructions on how to upload data are connected to a broken link. Sharing my data will happen by the end of my tenure as a graduate student in June 2023. These datasets will include .csv files, GIS map layers, and .Rmd files. These data will be as freely available as possible for reuse, redistribution and creation of derivatives with a CC0 licenses.


The length of time the data on the Clearing House website will be archived, maintained and preserved is unclear. Access to these data are limited in the sense that requesting it is required. The data shared in the Scholars Archive at OSU will require no maintenance and will be openly accessible. The data shared in this repository are preserved indefinitely. 


