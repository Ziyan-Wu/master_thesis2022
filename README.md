# Explore the utilization of ICESat-2 data in building height estimation area
*This is the repository for my master thesis in 2022*.


## What is ICESat-2?
<https://icesat-2.gsfc.nasa.gov/>

## Data Source
1. [ICESat-2](https://search.earthdata.nasa.gov/search)
2. [3D BAG](https://3dbag.nl/en/download)

## Library used  
see in `thesis.yaml`.

## Explaination
- **00h5togpkg**. 

This is to download the ICESat-2 data from offical website and convert it into .jpkg format. The used language is Julia.

- **01read**. 

This is to clip the two data, making it consistent with the municipal boundary. And also integrate the wanted layers from 3d BAG data. Store them as .gpkg or .geojson format.  

The boundary of municipal is downloaded from OpenStreet Map. Follow the [instruction](https://peteris.rocks/blog/openstreetmap-administrative-boundaries-in-geojson/) here. 

- **02explore**.

This is to explore the `confidence` attribute of the ICESat-2 data. Also incluing the data cleaning steps. The intersection analysis of ICESat-2 data and builidng's footprint is also in this file.

- **03ground_roof**. 

This is to classify the ground and roof ICESat-2 points. Including use interpolation methods to define the ground elevation and percentile method to define the roof elevation.
The interpolation is from [previous assignment code](https://github.com/Ziyan-Wu/geo1015/tree/master/hw_01/new)

- **04error**. 

Analyze the accuracy of the calculated result, including ground and roof elevation, building height. Compare it with reference value from 3D BAG.

- **ML part**.  

This folder includes the machine learning part.

- **Interplation**.  
Code from previous assignment (GEO1015 hw01)
