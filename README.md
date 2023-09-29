# Data
This repository is dedicated to data preparation for a case study on the QUANT Model in Shenzhen, China.

## DataPreprocessing.ipynb
This notebook encompasses data processing, fitting Beta, and the prediction of the Tij matrix, utilizing methods derived from Dr. Richard Milton’s QUANT model.

## sgh_geolist.geojson, shenzhen_sub_districts.geojson
sgh_geolist.geojson contains boundary data for the cities of Shenzhen, Dongguan, and Huizhou at the sub-district level, one of the administrative divisions of China.
shenzhen_sub_districts.geojson separately outlines the boundaries within Shenzhen alone, also at the sub-district level. Shenzhen comprises 61 sub-districts, with areas ranging from 168 square kilometers to 1.1 square kilometers.

## SGH_movement_Street_level.csv
Provided and preprocessed by China Unicom, one of the three major cellular carriers in China, this dataset includes specific commuter flow data for Shenzhen, Dongguan, and Huizhou. A place with the most prolonged stay from 09:00 pm-08:00 am is deemed as the probable residence, and if this stay exceeds 15 days a month, it is considered valid. Conversely, locations with the longest stay between 09:00 am and 05:00 pm are deemed workplaces. Commuting is identified as traveling from home to work. Individual commuting trips are consolidated at the street scale, creating links between streets within the study area. This dataset thus represents processed commuter flow data with 8921 pairs of Origin-Destinations (OD), detailing original and destination street ID, number of commuters, average commuting time, and distance.

## shenzhen_Tij_matrix.csv
This file contains flow data for Shenzhen extracted from SGH_movement_Street_level.csv and structured into matrix format, with the vertical axis indicating the origin ID and the horizontal axis indicating the destination ID.

## shenzhen_cij_matrix.csv
This matrix represents the Euclidean distances between various origins and destinations. Used to represent travel costs

## shenzhen_Tij_Predmatrix.csv
This file holds the predicted Tij matrix. The computations and code for these calculations are available in DataPreprocessing.ipynb.