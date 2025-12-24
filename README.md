# Remote Sensing Analysis for Urban Green and Blue Spaces

This repository contains the Google Earth Engine (GEE) JavaScript code used in the research paper "[Your Paper Title Here]" ([Journal Name, e.g., Submitted to *Nature Cities*]).

The scripts generate the core datasets used to analyze spatial disparities in green space (NDVI) and blue space (MNDWI) across 20 major global cities.

## 🗺️ Study Cities
The analysis covers the following cities, classified by the World Bank FY24 income group (HI, UM, LM):
- Tokyo (HI), New York (HI), Seoul (HI), London (HI), Paris (HI), Moscow (UM), Madrid (HI), Sydney (HI), Toronto (HI), Los Angeles (HI)
- Delhi (LM), Dhaka (LM), Karachi (LM), Lagos (LM), Kinshasa (LM)
- Cairo (UM), Jakarta (UM), Manila (UM), Sao Paulo (UM), Mexico City (UM)

## 📁 Repository Structure
- `scripts/`
  - `calculate_ndvi_mndwi_20cities.js`: Main script to extract Sentinel-2 imagery, calculate NDVI & MNDWI indices, and compute zonal statistics for each city.
  - `extract_population_data_20cities.js`: Script to extract gridded population count and density data from the GHS-POP dataset for each city boundary.
- `data/` *(optional - for sample outputs)*
  - `city_metrics_sample.csv`: Example table of the derived metrics (NDVI, MNDWI, population) for all cities.
- `README.md`: This file.

## 🚀 How to Use
1.  **Access Google Earth Engine:** You need a registered Google Earth Engine account.
2.  **Run the Scripts:**
    - Go to the [GEE Code Editor](https://code.earthengine.google.com/).
    - Copy the contents of a `.js` file from this repository.
    - Paste it into the Code Editor's script panel, modify the time period or export settings if needed, and click **Run**.

## 📊 Output Metrics
The primary scripts calculate the following for each city:
- **Urban Greenness:** Mean NDVI, percentage of vegetated area.
- **Blue Space:** Percentage of area covered by surface water (from MNDWI).
- **Population Context:** Total population and average density (persons/km²).

## 📚 Data Sources
- **Satellite Imagery:** Sentinel-2 MSI Level-2A, accessed via Google Earth Engine.
- **Population Data:** GHS-POP R2019A (GHSL), accessed via Google Earth Engine (`JRC/GHSL/P2016/POP_GPW_GLOBE_V1`).
- **City Boundaries:** Official administrative boundaries (source to be cited).

## 📄 License
This code is provided under the [MIT License](LICENSE) to support open and reproducible research.

## 🙋 Citation
If you use this code in your research, please cite our associated paper:
> [Your Full Paper Citation Will Appear Here]
