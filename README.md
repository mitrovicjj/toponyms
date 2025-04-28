# Toponym analysis project

## Overview
This project focuses on the analysis of toponyms (place names) across the former Yugoslav republics and surrounding regions. The dataset consists of geographic data, including toponyms with their respective latitudes and longitudes. The primary objective is to explore the linguistic and morphological aspects of the toponyms by cleaning and modifying the data, and clustering them based on their geographic proximity. Special attention was given to preserving the morphological roots of the toponyms by isolating suffixes and prefixes, which allowed for a better understanding of the name patterns within the dataset.

## Project structure
- **Data modification**: Starting with the cleaning process, where missing values are addressed. A key step involves handling the morphological structure of the toponyms. To ensure consistency and minimize noise, suffixes and prefixes are identified and separated. This allows for a focus on the core elements of the toponyms, such as their roots, which is essential for later classification and clustering. The names are normalized by eliminating irrelevant variations (e.g., 'ici', 'evici', 'ovci') to improve the clarity of the analysis.
  
- **Clustering with K-means**: After preprocessing the names, K-means clustering is employed to group toponyms that share geographic proximity. This step is crucial for identifying regions with similar linguistic characteristics, helping to discover patterns or trends that could be tied to historical, cultural, or geographical influences.

- **Semantic analysis**: Future directions include examining the semantic properties of toponyms by analyzing suffix patterns and their possible relationships to cultural or historical influences. The project is also considering advanced methods of classification based on linguistic features to explore how certain types of toponyms (e.g., surname-like names) behave across different regions.

- **Visualizations**: Although initial attempts at geospatial visualizations were made (using tools like GeoJSON), performance issues with the dataset size led to their exclusion. Future work will focus on finding efficient ways to visualize the data, potentially through selective sampling or exploring lighter mapping techniques.

## Dataset
The dataset used in this project is derived from GeoNames, focusing on toponyms in the following countries:
- Bosnia and Herzegovina
- Croatia
- Montenegro
- Serbia
- North Macedonia
- Bulgaria

The data contains the following columns:
- `geonameid`: Unique identifier for each location
- `name`: Name of the toponym
- `latitude`: Latitude of the location
- `longitude`: Longitude of the location
- `population`: Population of the location
- `elevation`: Elevation of the location
etc...


## Future Steps
- **Improved Clustering Techniques**: Explore other clustering algorithms, such as DBSCAN, that might better handle spatial data.
- **Toponym Classification**: Investigate methods to classify toponyms based on their suffixes or other linguistic features (e.g., surname-like toponyms).
- **Geospatial Visualizations**: Work on alternative ways to visualize the data, possibly by reducing the dataset size or exploring different visualization libraries that perform better with larger datasets.

## Acknowledgments
The geographic data used in this project is sourced from the GeoNames database. You can access more information at [GeoNames](https://www.geonames.org/).

