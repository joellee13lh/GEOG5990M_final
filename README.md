# GEOG5990M_final
fianl assignment of python module

# Manchester Housing Prices and Transport Accessibility Analysis

## Project Overview
This research explores the spatial relationship between house prices and public transport accessibility in the Greater Manchester metropolitan area. Using Geographically Weighted Regression (GWR), the analysis reveals significant spatial heterogeneity in how transportation accessibility influences property values across different neighborhoods.

## Data Sources
This project utilizes open data from multiple sources:

1. **Housing Price Data**: UK property transaction records (January-March 2025) from the [UK Government Price Paid Data](https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads#march-2025-data-current-month)

2. **Postcode Geographic Data**: Ordnance Survey Code-Point Open dataset providing precise postcode centroids, available from [OS Data Hub](https://osdatahub.os.uk/downloads/open/CodePointOpen)

3. **Public Transport Stops**: Bus, tram, train stations and airport location data

4. **Administrative Boundaries**: LSOA (Lower Layer Super Output Areas) boundary data for Greater Manchester

## Repository Structure
- `GEOG5990M_Final_Manchester_analysis.ipynb`: Jupyter notebook containing the complete analysis
- `README.md`: This file, providing project overview and instructions
- `/data/`: Directory containing smaller data files and links to larger files

## Large File Note
Due to GitHub's file size limitations, larger data files have been uploaded to Google Drive. The notebook contains code to automatically download these files using the following links:

- Housing Price Data: [pp-2025.csv](https://drive.google.com/file/d/1pwLMkWIKY2NeoM-r1l0LILYsHgjvki_M/view?usp=drive_link)
- Postcode Data: [codepo_gb.gpkg](https://drive.google.com/file/d/18-Ab0X8S252mAIGi564cSh4cqqctIpLi/view?usp=drive_link)
- LSOA Boundaries: [england_lsoa_2021.zip](https://drive.google.com/file/d/1-ITpRSqEKZZSwB9se26b2XHJ0qGCwaV5/view?usp=drive_link)
- Bus Stop Data: [Stops.csv](https://drive.google.com/file/d/1O5TD8zSmVXRmnklRfakBmyBN1hT34AEu/view?usp=drive_link)

## Analysis Methodology
The analysis follows these key steps:

1. **Data Preparation**: Filtering property transactions to Manchester area and cleaning transport data
2. **Spatial Processing**: Adding geographical attributes to house prices using postcode data
3. **Model Development**: Implementing GWR with transit-type weighted variables
4. **Visualization**: Creating both non-spatial (violin plots) and spatial (point-based maps) visualizations

## Key Findings
- Transport accessibility explains approximately 4.9% of house price variation globally, but up to 23.7% locally
- Significant spatial heterogeneity exists across Greater Manchester in how transit accessibility affects house prices
- Southern areas (particularly Stockport, Altrincham, Cheadle) show strong positive relationships between transport accessibility and house prices
- Urban core areas display weaker relationships, suggesting other amenities play more dominant roles there

## Running the Analysis
1. Clone this repository
2. Ensure you have the required dependencies: `pandas`, `numpy`, `geopandas`, `matplotlib`, `seaborn`, `contextily`, `statsmodels`, `scikit-learn`
3. Run the notebook: The first cell contains code to automatically download all required data files
4. Allow approximately 5-10 minutes for data processing and model execution

## References
The analysis builds upon established geospatial methodologies, including:
- Geographically Weighted Regression (Fotheringham et al., 2003)
- Transport accessibility impact studies (Banister, 2008; Debrezion et al., 2007)
- Spatial visualization best practices (Mennis, 2006; Crameri et al., 2020)

## Author
Student ID: 201896942——Zihao Li
