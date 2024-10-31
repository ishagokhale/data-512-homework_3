# data-512-homework_3

## Goal 
The goal of part 1 was to conduct a base analysis on impact of wildfires on a specific city. My assigned city was Dayton, Ohio. Part 1 is meant to allow us to explore: What are the estimated wildfire smoke impacts on your assigned city each year for the most recent 60 years of wildfire data? We create smoke estimates and compare them with AQI estimates over the last 60 years of available wildfire data. 


## Licensing and Source Data
The data for this project looks at the impact of wildfires, especially their effects on air quality in the western US. This dataset was collected and aggregated by the US Geological Survey. The dataset provides fire polygons in ArcGIS and GeoJSON formats. 
The source data is from https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81  

I used FIPS code, latitude and lognitudinal data for the city I was analyzing: Dayton, Ohio, which I got from its Wikipedia page linked here: nhttps://en.wikipedia.org/wiki/Dayton,_Ohio  

I found information on how to calculate AQI estimates through the following link: https://www.epa.gov/outdoor-air-quality-data/how-aqi-calculated  

I also used sample code in my notebookfrom Dr. David McDonald which is licensed through CC-BY, linked here:
https://creativecommons.org/licenses/by/4.0/

## Intermediary Files 
I have a json file of the filtered original data for wildfires within 1800 miles of Dayton. This file is too large for the repository, however. It has the following shcema:
```
{
        "attributes": {
            "OBJECTID": 14136,
            "USGS_Assigned_ID": 14136,
            "Assigned_Fire_Type": "Wildfire",
            "Fire_Year": 1962,
            "Fire_Polygon_Tier": 1,
            "Fire_Attribute_Tiers": "1 (1), 3 (1)",
            "GIS_Acres": 35.20257454524206,
            "GIS_Hectares": 14.245976488342759,
            "Source_Datasets": "Comb_National_NIFC_Interagency_Fire_Perimeter_History (1), Comb_National_NPS_Wildland_Fire_Perimeters (1)",
            "Listed_Fire_Types": "Wildfire (2)",
            "Listed_Fire_Names": "CHESTNUT (2)",
            "Listed_Fire_Codes": "No code provided (2)",
            "Listed_Fire_IDs": "1962-TNGSP-2007 (2)",
            "Listed_Fire_IRWIN_IDs": "",
            "Listed_Fire_Dates": "Listed Wildfire Discovery Date(s): 1962-05-06 (1) | Listed Wildfire Controlled Date(s): 1962-05-07 (1) | Listed Wildfire Out Date(s): 1962-05-14 (1) | Listed Other Fire Date(s): 2017-03-13 - NIFC DATE_CUR field (1) | Listed Upload Date(s): 2012-07-24 (1)",
            "Listed_Fire_Causes": "Natural (1)",
            "Listed_Fire_Cause_Class": "Undetermined (1), Natural (1)",
            "Listed_Rx_Reported_Acres": null,
            "Listed_Map_Digitize_Methods": "HeadsUp Digitized (1)",
            "Listed_Notes": "",
            "Processing_Notes": "",
            ...
            "Shape_Length": 1627.4165754908233,
            "Shape_Area": 142459.7648834276
        },
        "geometry": {
            "rings": [
                [
                    [
                        1056046.4017000012,
                        ...
                    ]
                ...
                ]
            ...
            ]
        ...
        }
}
```

