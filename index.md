# 1. Data description

This research is concerning steelhead salmon and the habitat they occupy in various Oregon watersheds. In this project we will be addressing questions regarding the relationship between different habitat characteristics, how changes in these habitat variables may impact steelhead populations, and how valuable some methods of data collection are compared to others in understanding these fish. 
we will be using existing datasets which have already been collected by others from Oregon Department of Fish and Wildlife (ODFW). These data include:

- Surveys and describe various components of steelhead habitat along streams in Oregon as well as population data for each species. This was collected using a Generalized Random Tessellation Stratified (GRTS) survey. These data exist as tabular data stored in multiple .csv files.
- *VELMA (Visualizing Ecosystem Land Management Assessments) inputs*:
VELMA models will be re-run for the period of ODFW Aquatic Inventories (AQI) habitat data (1998 – 2020) while also including the novel, and complimentary model, PENUMBRA (model that can produce spatial and temporal representations of shade percentage and ground-level solar energy), to also export modeled stream temperature values. Stream temperature values will be validated with ODFW thermistors where and when available. All spatial data to run these models has been collected and organized. Only weather data (daily precipitation and daily air temperature) is needed. These data will be obtained from the PRISM climate group (https://prism.oregonstate.edu/). 

- *VELMA outputs*:
Outputs of the VELMA model (daily stream flow and temperature GIS layers) will be validated against USGS stream gage data using the Nash-Sutcliffe efficiency co-efficient (NSE) while instream temperature will be validated against thermistors with seasonal simulated-observed metrics.

All of these data will be useful in developing species distribution models for juvenile steelhead salmon. Species distribution models (SDM) use multiple covariates to project the presence or absence of individuals. This model will be used to describe the productivity and suitability of juvenile steelhead habitat and to guide targeted habitat management actions. We will use these habitat data and modeled covariates to inform the SDM. We will assess the most influential habitat characteristics in determining the likelihood of presence or absence, by running a series of general additive models. These models will be run using R. The SDM will be developed using R. Both of these will be connected to the graduate student's GitHub.
	
Currently there is approximately 1-2 GB of datasets, as we develop GIS projects and layers this number will increase to 3-4 GB or more.  
  
# 2. Roles and Responsibilities

The PI will be responsible for implementing the DMP. Because this project is based on existing data, a dimension of the graduate student's work will include acquiring, organizing, storing, and analyzing these data sets. Therefore, the graduate student will be solely responsible for these tasks as well as developing a system of archiving both the data and future analyses. Metadata is largely not included in the datasets currently and because of this the graduate student will continue to contact the original owners of the data to generate and ammend any missing metadata. ODFW include raw fine scale habitat data for steelhead as well as population data. All of the from ODFW have copies with the original owners. These datasets are unrestrictive and do not contain sensitive information.

While this project has many partners, the graduate student has sole responsibility over developing and applying this data management plan. If the graduate student were to suddenly leave this project, the responsibilities of the student would fall to the PI. Since the graduate student will be using data collected by other people,  copies will be made of all of these datasets and stored in a separate folder of the Box drive that is shared with all project partners prior to future analysis. The original copies exist with the original owners who are at ODFW. The owners of the Box drive are the PI as well as our partners at ODFW, therefore information will not be lost after the graduate finishes on this project. The Box drive will be the sole location for all data, however for data which is larger (i.e. VELMA model outputs) these will be exchanged through a hard drive which is the property of OSU. This is to share the data within the project, however the original outputs belong to ODFW. All datasets will be stored as .csv to ensure accessibility and all analyses will be accessible through RStudio, and open source platform. All spatial data layers will be stored together as zip files to ensure that all of the necessary data to view the layers is together. 

As this project continues we will develop models to analyze the population and habitat data. I hope to develop a package in R to store these methods of analysis as well as the metadata behind each step within the models. We will include all of this information as well as instructions of reproducibility within the package help files. 


# 3. Data Standards and Metadata

## Habitat and Abundance Data
This project will be using tabular data from habitat and population surveys which have already been collected by other individuals at ODFW. These data exist in multiple .csv files which will be analyzed using R in R studio. These surveys are stored as tabular data and will include a readme sheet which stores the definitions of variables as well as contact information for those who collected the data.The graduate student will create duplicates of all .csv files that are adjusted as well as describing any changes in the readme. The naming convention for each data set will include date edited (in year_month_day),datadescription (i.e. habitatdata). To ensure that the changes made to dataset format, as well as new data developed through these various analyses, we will implement the file naming convention referenced above as well a visual guide for the DMP. This visual guide will display the location of files, the system of organization, as well as the contact information for those who are associated with the data who may be helpful resources. 

## Coding
New datasets will be generated as we continue with this project. This will include analyses being applied to the tabular data described above, and being executed in R studio. Progress in R studio will be documented by using GitHub. GitHub will be an essential tool in data version control.  

Another dimension of this research will be developing an R package that will be a specific group of functions to run a species distribution model with this data. The documentation of developing the R package will be as described above, and will also be included in the specific help file for the package and each of the functions. The data we use will also be callable from the package itself once the package is installed. 

## Geospatial Metadata
We will utilize the software ArcGIS Pro and create geodatabases where relevant data will be stored as ‘projects’ including readme.md files. In compliance with Federal Geographic Data Committee's standards will be in the Unified Modeling Language (UML). The metadata will contain: metadata record information (i.e. language it is written in, unique identifier, relavant contact information), appropriate maintenance information, and spatial representation. 

# 4. Storage and Security
## Storage

_Box Drive_

- Literature reviewed as tabular data.
- Habitat and abundance data (i.e. tabular data, GIS layers).
- Backup strategy: downloading Box drive to graduate student's laptop.

_External hard drive_

- Transferring VELMA model outputs between devices.
- Backup strategy: Copies of these outputs exist with ODFW colleagues and will be saved to Box drive by graduate student.

_GitHub_

- Graduate student will perform analysis using their personal GitHub.
- Backup strategy: Download archive and upload to Box drive.
	
## Security
There is no sensitive information or data which needs extrodinary security measures. 

# 5. Access and Data Sharing

These data will be made publicly available and are not sensitive with any need for protection or security measures. Some datasets will only be available for future use, redistribution, and creating derivatives upon request to current associates of ODFW and OSU. Data analyzed, published, and preserved by the graduate student will be available through the OSU data depository, ScholarsArchive@OSU: https://ir.library.oregonstate.edu/.


# 6. Archiving and Preservation 


There are no requirements for data management, release, or preservation for this project. Any products of the graduate student's own research including GIS layers, mathematical models used for analysis, written reports, and other datasets will be publicly available in the OSU data depository, ScholarsArchive@OSU:
https://ir.library.oregonstate.edu/

The release of these data will occur by the end of the tenure of the graduate student in Fall 2023. These datasets will include .csv files, GIS map layers, and .Rmd files. These data will be as freely available as possible for reuse, redistribution and creation of derivatives with a CC0 licenses.
	The data shared in the Scholars Archive at OSU will require no maintenance and will be openly accessible. The data shared in this repository are preserved indefinitely. Copies of the mathematical models and other analysis will be stored in the graduate student's personal GitHub and files will remain in the Box drive for at least 3 years after the graduate student is no longer on the project. These files can be made available upon request of the PI and ODFW partners. 


