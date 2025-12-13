## About

This repository contains files for the 'Working with Environmental Datasets' course (EDS 220), Homework 4, task 2. The Jupyter notebook `hwk4-task2-false-color-Morquecho.ipynb` contains a Python analysis and visualization of the data mentioned below using false and true color imagery to show the burn areas of the January 2025 Palisades & Eaton fires in California. The notebook `eaton-palisades-fires-EJI-Kaiju-Morquecho.ipynb` contains the analysis of the burn areas using the Environmental Justice Index.

### Repository Structure 
```
├── .gitignore
├── hwk4-task2-false-color-Morquecho.ipynb
├── eaton-palisades-fires-EJI-Kaiju-Morquecho.ipynb
├── README.md
```
### Purpose

The purpose of this repository is to use `netCDF4` data files, accessed with the `xarray` library, to visualize the burn scars from the Eaton and Palisades fires that occurred in January of 2025, within the context of environmental exposures, underlying health conditions, and socioeconomic vulnerability of the affected communities. 

### Highlights
- Use the `xarray` library to streamline analysis of `netCDF4` files containing multidimensional data
- Use false color imagery to highlight burn areas after California wildfires 
- Address common remote sensing data issues such as extreme and `np.nan` values that distort data visualizations

### About the Data
- Fire perimeter data are sourced from the [eGIS LA County hub](ttps://egis-lacounty.hub.arcgis.com/maps/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/about), and can be accessed and downloaded by selecting the desired layer and clicking 'Download'. Dataset for the layer `Eaton_Perimeter_20250121` contains the `.shp` file of the Eaton Fire dissolved perimeter, while `Palisades_Perimeter_20250121` contains the Palisades Fire dissolved perimeter. Both datasets are in the `EPSG:3857` `CRS`.

- Landsat data was provided by the course instructor, Dr. Carmen Galaz Garcia, as a simplified collection of bands (red, green, blue, near-infrared, and shortwave infrared). The data comes from the Landsat Collection 2 level-2 atmospherically corrected surface reflectance data, which is collected by the Landsat 8 satellite. The original data and other related datasets can be retrieved from the [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2). The data is in the `EPSG:32611` `CRS`.

- The Environmental Justice Index (EJI), produced by the Centers for Disease Control and Prevention and the Agency for Toxic Substances and Disease Registry, provides nationwide measures of cumulative environmental, social, and health burden at the census tract scale. The dataset combines indicators related to environmental exposures, underlying health conditions, and socioeconomic vulnerability to identify communities that may face disproportionate environmental and health risks. The data can be accessed and downloaded from the [CDC website](https://atsdr.cdc.gov/place-health/php/eji/eji-data-download.html). The data is in the `EPSG:4269` `CRS`.

### References
Los Angeles County GIS. (2025). Palisades and Eaton Dissolved Fire Perimeters (2025) [Data layer]. eGIS LA County Hub. https://egis-lacounty.hub.arcgis.com/maps/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/about. Accessed November 22, 2025, via ArcGIS: https://www.arcgis.com/home/item.html?id=ad51845ea5fb4eb483bc2a7c38b2370c

Earth Resources Observation and Science (EROS) Center. (2025). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6. Accessed November 22, 2025, via Microsoft Planetary Computer: https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2.

Centers for Disease Control and Prevention and Agency for Toxic Substances Disease Registry. (2025) Environmental Justice Index. Accessed November 28, 2025: https://atsdr.cdc.gov/place-health/php/eji/eji-data-download.html

Galaz Garcia, C., & Adams, A. (2025). EDS 220: Working with environmental datasets [Course website]. University of California, Santa Barbara, Master of Environmental Data Science Program. https://meds-eds-220.github.io/MEDS-eds-220-course/
