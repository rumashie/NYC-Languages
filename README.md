# NYC Community Language Profiles Map
NYC Open Data Visualized 

This project is a recreation of an existing NYC Community Language Profiles Map using Python and various geospatial libraries. The original project utilized technologies that I was not familiar with, and this recreation aims to implement the map using languages and technologies I am proficient in.

view project here: 
https://nbviewer.org/github/yomashie/NYC-Languages/blob/main/nyc_OpenData.ipynb


## Libraries Used
- pandas
- folium
- geopandas
- numpy

## Data Source
The data for this project is sourced from Open Data NYC. Specifically, two datasets are used:
1. `NYC Community Language Profiles.csv`: Contains language profiles for different community districts in NYC.
2. `Community_Districts.json`: GeoJSON file containing geographical information about NYC community districts.

## Code Overview
The main script ('nyc_OpenData.ipynb') performs the following tasks:

1. **Data Loading and Merging:**
   - Loads language profile data from `NYC Community Language Profiles.csv`.
   - Loads geographical data from `Community_Districts.json` and renames the necessary columns.
   - Merges the two datasets based on the "Borough CD Code."

2. **Map Creation:**
   - Creates a folium map centered at (40.75, -74.125).
   - Adds a choropleth layer depicting the percentage of the population with Limited English Proficiency.

3. **District Division:**
   - Divides the map into districts using GeoJson.

4. **Hover Functionality:**
   - Implements hover functionality to display information about each community district.

5. **Parks Highlight:**
   - Highlights parks on the map

6. **Dark and Light Modes:**
   - Adds toggleable dark and light modes using different tile layers.

7. **Layer Control:**
   - Includes a layer control for easy toggling of map layers.

## Acknowledgments
- Data provided by Open Data NYC.

