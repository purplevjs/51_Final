

# Duke University Air Pollution and Health Dataset

Overview

This dataset provides information about air pollution levels and health outcomes in the Duke University region. It includes satellite-derived pollutant data for NO2 and PM2.5, along with synthetic health data related to asthma rates. The dataset is intended to help researchers, policymakers, and community stakeholders better understand the relationship between air quality and respiratory health in the area.

Motivation

The motivation behind this project is to explore the impact of air pollution on public health, focusing on the Duke University region. By analyzing pollutants like NO2 and PM2.5 and correlating them with health metrics such as asthma rates, the dataset aims to support evidence-based policymaking for air quality improvement. It also highlights the potential of satellite data to enhance our understanding of local health outcomes.

Data Description

Pollutants: The dataset contains concentrations of Nitrogen Dioxide (NO2) and Particulate Matter (PM2.5), collected using Google Earth Engine from satellite imagery (Sentinel-5P and MODIS).

NO2: Derived from Sentinel-5P, representing tropospheric NO2 column density.

PM2.5: Proxied using aerosol optical depth from MODIS imagery.

Health Metrics: Synthetic health data, including asthma rates for the selected region, has been added to explore correlations between air quality and respiratory health outcomes.

Data Collection Process

Satellite Data: Collected from Google Earth Engine, using image collections from Sentinel-5P and MODIS.

Time Period: The data covers the period from January 2022 to December 2023, ensuring coverage across different seasons.

Region: The geographic focus is on the Duke University region, with an expanded bounding box to cover Durham and surrounding areas.

Grid Analysis: The region is divided into subregions to calculate average pollution levels, allowing for spatial analysis of pollutant concentrations.

Tools Used

Google Earth Engine (GEE): For retrieving satellite data.

Rasterio: For processing and analyzing the pollutant GeoTIFF files.

Pandas: For creating and managing the dataset.

Hugging Face Datasets: To host the dataset and make it publicly available.

License

This dataset is licensed under the CC BY 4.0 license, allowing for reuse with attribution. Users are encouraged to cite this dataset if used for research or other public purposes.

Ethics Statement

The data is derived from publicly available satellite sources and does not contain any personally identifiable information (PII).

Health data provided is synthetic and meant solely for analytical purposes to explore correlations.

How to Use This Dataset

This dataset can be used for:

Exploratory Analysis: Understand the spatial distribution of air pollutants and their potential health impacts.

Policy Support: Provide evidence for local health authorities and policymakers to improve air quality management.

Machine Learning Models: Train models to predict health outcomes based on pollution data.

Dataset Statistics

Number of Subregions: Divided into multiple subregions of 5x5 grids for fine-grained analysis.

Variables: NO2 levels, PM2.5 levels, and synthetic asthma rates.

Example Usage

from datasets import load_dataset

Load the dataset from Hugging Face Hub
dataset = load_dataset("Violetjy/duke_pollutants_health")

Display the first few rows
print(dataset["train"].to_pandas().head())

Acknowledgments

Special thanks to Google Earth Engine for providing access to satellite imagery, and to the Hugging Face team for hosting the dataset.

Citation

Please cite this dataset as:

"Duke University Air Pollution and Health Dataset, 2024, created by Violetjy. Available at Hugging Face Datasets Hub."

For further questions or feedback, feel free to reach out!
