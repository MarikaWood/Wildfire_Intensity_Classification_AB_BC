# Classification of Wildfire Intensity in Alberta and British Columbia Using Satellite and Environmental Data
This repository contains th code used for the data preprocessing, dataset construction, and maching learning modeling described in the capstone project:
**Classification of Wildfire Intensity in Alberta and British Columbia Using Satellite and Environmental Data**
The project explores the environmental conditions associated with high-intensity wildfire activity in Western Canada by integrating satellite fire detections with meteorological and land cover data.

---

## Project Overview

Wildfires are a recurring natural hazard in Alberta and British Columbia with significant environmental, economic, and societal impacts. Understanding the environmental conditions associated with high-intensity wildfire activity can support improved wildfire risk assessment and preparedness.

This project combines three open-source datasets:

- **VIIRS satellite fire detections**
- **Meteorological station observations**
- **MODIS land cover classifications**

These datasets are integrated to construct classification-ready datasets used to predict high-intensity wildfire activity using machine learning models.

The analysis evaluates multiple classification approaches including:

- Logistic regression
- Random forest
- Logistic regression and random forest ensemble modeling

Model performance is evaluated using standard classification metrics including precision, recall, and ROC–AUC, with emphasis on predicting high-intensity fire activity.

---

## Repository Structure

- **notebooks/**
  - **preprocessing/** – fire data preprocessing and dataset construction
  - **modeling/** – machine learning model implementation and evaluation

- **data/**
  - documentation for datasets used in the project

### Preprocessing notebooks

These notebooks construct the modeling datasets from the original satellite and meteorological observations. The preprocessing workflow includes:

- Fire detection preprocessing and aggregation
- Meteorological dataset preparation
- Land cover enrichment
- Dataset merging and validation
- Exploratory data analysis and Fire Radiative Power (FRP) threshold selection
- Finalization of model-ready datasets

### Modeling notebooks

These notebooks implement and evaluate the classification models used in the project:

- Logistic regression classification models
- Sensitivity analysis based on meteorological station distance
- Random forest classification models
- Spatial sensitivity analysis excluding geographic predictors
- Logistic regression and random forest ensemble modeling

---

## Data Sources

The datasets used in this project were obtained from publicly available sources.

### VIIRS Fire Detection Data

VIIRS S-NPP 375 m Active Fire Product  
NASA FIRMS / Earthdata

https://earthdata.nasa.gov/

### Meteorological Data

Environment and Climate Change Canada (ECCC)  
MSC Datamart historical climate data

https://www.canada.ca/en/environment-climate-change/services/weather-general-tools-resources/weather-tools-specialized-data.html

### Land Cover Data

MODIS MCD12Q1 Land Cover Type Product (Collection 6.1)  
IGBP land cover classification system

https://doi.org/10.5067/MODIS/MCD12Q1.061

---

## Data Availability

Due to file size limitations, the full raw and processed datasets are not included in this repository. The notebooks in 'notebooks/preprocessing/' contain the full workflow used to construct the modeling datasets from the original data sources.

---

## Reproducibility

All data preprocessing, integration, and modeling steps described in the project report are implemented in Python using Jupyter notebooks. The repository is organized to reflect the workflow described in the report, allowing the analysis to be reproduced once the datasets are obtained from the sources listed above.

---

## Author

Marika Wood
