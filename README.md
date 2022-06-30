# Explore the utilization of ICESat-2 data in building height estimation area

## What is ICESat-2?
<https://icesat-2.gsfc.nasa.gov/>

## Data Source
1. ICESat-2
2. 3D BAG <https://3dbag.nl/en/download>

## Explaination
- **00h5togpkg**. 

This is to download the ICESat-2 data from offical website and convert it into .jpkg format. The used language is Julia.

- **01read**. 

This is to clip the two data, making it consistent with the municipal boundary. And also integrate the wanted layers from 3d BAG data. Store them as .gpkg or .geojson format.  

The boundary of municipal is downloaded from OpenStreet Map. Follow the [instruction](https://peteris.rocks/blog/openstreetmap-administrative-boundaries-in-geojson/) here. 

- **02explore**. 

This is 

- **03ground_roof**. 



This is the repository for my master thesis in 2022.
