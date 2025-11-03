x## GENERAL INFORMATION

* **Title of Project:** Evaluating Solar Canopy Potential for Renewable Energy Transition in Calgary's Urban Environment

# Author Information
- **Name:** Amelia Frazee  
- **UCID:** 30218310  
- **Institution:** University of Calgary  
- **Email:** amelia.frazee@ucalgary.ca  



# PROJECT OVERVIEW AND PURPOSE

This project evaluates where solar canopy systems could be most effective in Calgary by analyzing parking lots, building footprints, and solar exposure. The goal is to support renewable energy transition strategies in urban areas.



# FOLDER STRUCTURE GUIDE

- **FRAZEE_Solar_Suitability_Project_Data.gpkg.zip** – contains all spatial layers and attribute tables for analysis  
- **LICENSE** – licensing information for the dataset  
- **README.md** – project documentation  



# CRS AND DATA FORMAT NOTES

## Coordinate Reference System (CRS) 
All spatial data are projected using **WGS 1984 Web Mercator (Auxiliary Sphere)**.  

## Data Format
All spatial data are stored in **GeoPackage (.gpkg)** format to maintain attribute tables and spatial integrity.



# DATA SOURCES

Calgary_Latest_Orthophoto - ArcGIS Online
Off-street_Parking_Zones - Open Calgary
Digital elevation Model Lidar ASCII 2m - Open Calgary


**Data Collection Notes:**  
- Data were downloaded from Open Calgary and ArcGIS Online.  
- All Datasets were Open Source



# METHODS INFORMATION
- Imported spatial data from ArcGIS Online and Open Calgary into ArcGIS Pro 3.2
- Converted Off street parking zones into a new feature class and excluded incompatible sites  
- **Criteria evaluated** (weighted for MCDA):  
  - **Size ** – 25%  
  - **Proximity to electrical substations** – 25%  
  - **Grid hosting capacity** – 20%  
  - **Orientation / Shading** – 30%  
- Calculated a **Final_MCDA_Score** for each site (1–5 scale)  
- **Top-priority sites** identified using percentile thresholds of MCDA overall scoring  
- **Outputs:**  
  - Geodatabase with all attributes  
  - Excel table of scores  
  - 5 jpeg maps exported
- **Key tools used:** Near, Extract by Mask, Aspect, Reclassify, Zonal Statistics at Table, Python within ArcGIS for the field calculations
   - Attribute tables were cleaned and exported for reference in **Excel**.  



# DATA-SPECIFIC INFORMATION

### FRAZEE_Solar_Suitability_Project_Data.gpkg.zip  
- **Missing Data Codes:** `NULL` indicates missing values  



# SHARING / ACCESS INFORMATION

- **License:** Creative Commons Attribution 4.0 (CC-BY 4.0)  
- **<a href="https://example.com">Evaluating Solar Canopy Potential For Renewable energy Transition in Calgary's Urban Environment</a> © 2025 by <a href="https://example.com">Amelia Frazee</a> is licensed under <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"> **  
  
*https://github.com/ameliafraz/GEOG587_Project

