# Legazpi OSM Extracts and Polygon Boundary

This repository provides OpenStreetMap (OSM) data extracts and a polygon boundary file for **Legazpi City, Albay Province, Philippines**.  
It is primarily prepared for use with **[LAKBAI](https://github.com/johannbuere/LAKBAI)** — *An AI-Powered Tourist Navigation and Recommendation System for Legazpi*.



### Why this repository exists

The **LAKBAI project** requires accurate geospatial data to enable routing, navigation, and location-based recommendations.  
To power the OSRM (Open Source Routing Machine) backend, we need both:

- **Polygon boundary files** – to clip and define the geographic area of interest (Legazpi City).  
- **OSM extracts** – to provide the actual road network and map data for routing.

This repository serves as the dedicated source of those geospatial files, making it easier to maintain and reuse them across the project.


## Contents

The following files are included:

- **`legazpi.poly`**  
  Polygon boundary file for Legazpi City. Used to clip OSM data to the exact city limits.  

- **`albay.osm.pbf`**  
  OSM extract covering the entire Albay Province.  
  - Taken from the companion repository: [**albay-osm-extract**](https://github.com/johannbuere/albay-osm-extract)  
  - Extracted from `philippines-latest.osm.pbf` (downloaded via [Geofabrik](https://download.geofabrik.de/asia/philippines.html))  
  - **Updated as of 2025-08-18**  

- **`legazpi.osm.pbf`**  
  OSM extract clipped specifically to Legazpi City using the `.poly` boundary.  
  Optimized for city-level routing.



## Usage

These files can be used for:

- **OSRM (Open Source Routing Machine)** – Building a routing engine tailored to Legazpi City.  
- **Map rendering** – Visualizing the Legazpi area in map applications.  
- **Geospatial analysis** – Performing spatial queries, network analysis, or urban studies.  



## Data Sources

- **OpenStreetMap data** downloaded from [Geofabrik: Philippines extract](https://download.geofabrik.de/asia/philippines.html)  
- **Albay OSM Extract** maintained in: [albay-osm-extract](https://github.com/johannbuere/albay-osm-extract)  



## Related Project

- [**LAKBAI**](https://github.com/johannbuere/LAKBAI) – The main project that uses these data files.  
  *LAKBAI is an AI-powered tourist navigation and recommendation system designed for Legazpi City, helping visitors explore efficiently while discovering local attractions.*



## License

- **OSM Data**: © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright).  
  Licensed under the **Open Database License (ODbL)**.  

- **Polygon and derived extracts**: Same license as OSM data (ODbL).  
  Attribution is required if used in other projects.  

- **This repository**: Licensed under the MIT License for the repository structure and documentation.  
  Data files remain under ODbL as noted above.
