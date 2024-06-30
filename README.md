# Kyiv Store Population Analysis

This project aims to analyze the population distribution in Kyiv and identify optimal locations for new stores to maximize population served. The analysis is conducted using clustering techniques and visualized through interactive maps.


## Data

- **raw**: Contains raw data files.
  - `Population.csv`: Buildings in Kyiv with coordinates and population.
  - `Stores.csv`: Stores in Kyiv with coordinates and a metric.

- **processed**: Contains processed data files.
  - `Building_Store_Distances.csv`: Distances between buildings and existing stores.
  - `Population_with_Nearest_Store.csv`: Population data with nearest store information.
  - `Stores_with_Population_Served.csv`: Stores with population served metrics.
  - `distances_new_stores.csv`: Distances between buildings and potential new stores.
  - `new_stores_population_served.csv`: Potential new stores with population served metrics.

## Notebooks

- `Kyiv Store Population Analysis.ipynb`: Analysis of the population distribution and existing stores.
- `Optimal New Store Locations.ipynb`: Identification of optimal new store locations using clustering.

## Results

- **notebooks in html**: HTML versions of the notebooks.
  - `Kyiv Store Population Analysis Notebook.html`
  - `Optimal New Store Locations Notebook.html`
- `kyiv_population_map_1_km.html`: Interactive map showing population distribution within 1 km and existing stores.
- `kyiv_population_map_500_meters.html`: Interactive map showing population distribution within 500 meters and existing stores.
- `kyiv_new_store_locations_map.html`: Interactive map showing potential new store locations.
- `kyiv_new_store_potential_population.html`: Interactive map showing potential new store locations and population served.

## Guide to Using the Cluster Map: kyiv_new_store_locations_map

### Overview

The cluster map visualizes potential new store locations based on population distribution in Kyiv, helping stakeholders identify optimal store sites to maximize population served.

### Key Features

1. **Cluster Visualization**:
    - **Building Points**: Represented by circle markers, with size proportional to the building's population.
    - **Cluster Colors**: Color-coded for easy visualization.
    - **Tooltip Information**: Displays metric population, nearest new store ID, and distance to nearest new store.

2. **New Store Locations**:
    - **Markers**: Custom icons show rank by population served.
    - **Popup Information**: Includes new store ID, population served, and ranks within 1 km and overall.

### Usage Instructions

1. **Building Points**:
    - Gauge population size by circle size.
    - Use tooltips to see distance and cluster information.

2. **New Store Locations**:
    - Identify high-ranking locations.
    - Compare potential locations using popup details.

3. **Strategic Decision-Making**:
    - Identify underserved high-density clusters.
    - Prioritize locations serving the highest population within 1 km.

### Considerations

1. **Clustering Nuances**:
    - **Cluster Centers**: K-Means algorithm centers may be influenced by distant buildings.
    - **Distance Constraints**: The 1 km threshold ensures stores are within convenient walking distance.

2. **Business Impact**:
    - **Maximizing Reach**: Strategically placed stores serve more people effectively.
    - **Data-Driven Decisions**: Provides a robust, data-driven approach to selecting new store locations.

3. **Future Enhancements**:
    - **Continuous Monitoring**: Regular updates to population data and re-analysis.
    - **Advanced Clustering**: Explore other techniques for improved precision.

## Installation

To run the analysis, ensure you have all required packages installed. You can install the necessary packages using the provided `requirements.txt` file:
pip install -r requirements.txt
Also, update the output paths in the notebook files.