# Analysis of Changes to the BII in Maricopa County, Arizona
This repoistory contains the code and data for the analysis of BII (Biodiversity Intactness Index) changes within the Phoenix metro area in Maricopa County, Arizona. 

## About
In 2021, Maricopa County, home to the Phoenix metro area, was identified as the fastest sprawling county in the United States with the most signifcant increase in developed land since 2001. This rapid increase in urbanization is expected to have a profound impact on the biodiversity and health of nearby ecosystems.

This analysis investigates the impacts of urban sprawl on BII in the Phoenix Subdivision of Maricopa County between 2017 and 2020. In particular, this analysis will involve:
- Using an API to load data
- Manipulating raster data with rioxarray
- Manipulating raster data through raster math

## Repository Structure
```bash
├── README.md
├── .gitignore
├── data
│   └── tl_2022_04_cousub
│       ├── tl_2022_04_cousub.cpg
│       ├── tl_2022_04_cousub.dbf
│       ├── tl_2022_04_cousub.prj
│       ├── tl_2022_04_cousub.shp
│       ├── tl_2022_04_cousub.shp.ea.iso.xml
│       ├── tl_2022_04_cousub.shp.iso.xml
│       └── tl_2022_04_cousub.shx  
└── bii-changes-maricopa-county.ipynb
```

## Data
Biodiversity Intactness Index (BII) Time Series: Raster data depicting the intactness of biodiversity. This data is avaliable through the Microsoft Planetary Computer STAC catalog. The SpatioTemporal Asset Catalog (STAC) is a new standard for geospatial data, particulary for satellite imagery. To obtain data from a STAC catalog, we use an Application Programming Interface (API). The API acts as an intermediary between the STAC catalog and ourselves.

Phoenix Subdivision Shapefile: Shapefile of the Phoenix Subdivision as a subset of the larger shapefile of Arizona county subdivisions. This data is housed within the repository. Obtained from the United States Census Bureau.

## References
2022 TIGER/Line® Shapefiles: County Subdivisions, US Census Bureau, Geography Division. (2022). https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2022&layergroup=County+Subdivisions. [Accessed: Dec. 4, 2024]

Biodiversity Intactness, Microsoft Open Source, Matt McFarland, Rob Emanuele, Dan Morris, & Tom Augspurger. (2022). microsoft/PlanetaryComputer: October 2022 (2022.10.28). Zenodo. https://doi.org/10.5281/zenodo.7261897. [Accessed: Dec. 12, 2024]

F. Gassert, J. Mazzarello, and S. Hyde, “Global 100m Projections of Biodiversity Intactness for the years 2017-2020 [Technical Whitepaper].” Aug. 2022. Available: https://ai4edatasetspublicassets.blob.core.windows.net/assets/pdfs/io-biodiversity/Biodiversity_Intactness_whitepaper.pdf

Z. Levitt and J. Eng, “Where America’s developed areas are growing: ‘Way off into the horizon’,” The Washington Post, Aug. 2021, Available: https://www.washingtonpost.com/nation/interactive/2021/land-development-urban-growth-maps/. [Accessed: Nov. 22, 2024]

*Special thank you to Professor Carmen Galaz García and her course materials from EDS220*
