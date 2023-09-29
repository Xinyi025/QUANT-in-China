# Data

The repository is the data preparation about the case study in Shenzhen, China of QUANT Model. 

## sgh_geolist.geojson, shenzhen_sub_districts.geojson
sgh_geolist.geojson is the boundary files about the Shenzhen, Dongguan and Huizhou Cities, spatial scale is sub-district level (one of the administrative divisions of China). 
shenzhen_sub_districts.geojson is the boundary files about the Shenzhen, which is separate from sgh_geolist.geojson. Spatial scale is also sub-district level. Shenzhen has 61 sub-distrcits, and area ranges from 168 square kilometers to 1.1 square kilometers.

## SGH_movement_Street_level.csv
It is data provided by China Unicom, which is one of the top three cell phone carriers in China. This data is preprocessed by data provider. Specifically, the site with the most prolonged stay during the observation period (09:00 pm-08:00 am) in a day is considered as the candidate place of residence. When a candidate residence lasts for more than 15 days in a month, it is deemed to be valid. Similarly, the location with the most prolonged stay between 09:00 am and 05:00 pm is determined to be the workplace. Commuting is defined as a journey from one's home to the workplace. Individual commuting trips of mobile phone users are aggregated at the street scale, generating links between streets across the study area (SDH region).
## shenzhen_Tij_matrix.csv

