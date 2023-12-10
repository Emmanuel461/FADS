###**Metada of satellite and raster files**

The files of climate data was obtained from: https://www.worldclim.org/data/index.html 

In this case the information and units of the retrieved was:


| Variable                        |Units         |Spatial resolution |  
|---------------------------------|--------------|-------------------|
| Precipitation                   |  mm          | 1km               |  
| Monthly minimum temperature     |  °C          | 1km               |  
| Monthly maximum temperature     |  °C          | 1km               |  
| Monthly mean temperature        |  °C          | 1km               |  
| Solar radiation                 | kJ m-2 day-1 | 1km               |  

 *Data retrieved from: (Fick, S.E. and R.J. Hijmans, 2017).*

The optic data was retrieved from Google Earth Engine, the source code is:
https://code.earthengine.google.com/26ee28c0e17b34f5f388ff07fa311d1c

The selected sensor for this project was Sentinel-2. The characteristics of the sensor are:

| Metadato                | Valor                                      |
|-------------------------|--------------------------------------------|
| Satellite name    | Sentinel-2                                 |
| Number of bands         | Banda 1, Banda 2, ..., Banda 12             |
| Resolución espacial     | 10 meters (Band 2, Band 3, Band 4)       |
|                         | 20 meters (Band 5, Band 6, Band 7, Band 8A)|
|                         | 60 meters (Band 1, Band 9, Band 10, Band 11, Band 12)|
| Temporal resolution     | 5 days$_{1}$                            |
| Adquisition date  | From 2022-01-01 to 2022-12-31                     |
| Orbit                  | Número de la órbita                        |
| Processing level  | Level-1C, Level-2A$_{2}$ , Level-2                   |
| Retrived data from |Google earth engine           |
| Coordinate system  | WGS 84                                     |
| File Formt      | GeoTIFF                     |
| Data provider      | Copernicus                                 |
| Optional download URL        | https://scihub.copernicus.eu/                   |

[1]This is the process level used in this project
[2]This is the temporal resolution of the sensor, the number of images was not all in the showed period because the images with the high rate of clouds were excluded. 

The raster layers of digital elevation model (DEM) was the digital elevation-shuttle radar topography mission (SRTM): 

| Metadato                | Valor                                      |
|-------------------------|--------------------------------------------|
| Mission                  | Shuttle Radar Topography Mission (SRTM)     |
| Entity Id                | SRTM1N11W016V3                              |
| Data Source         | Radar de apertura sintética (SAR)          |
| Spatial resolution     | Aproximadamente 30 metros (1 arco segundo)|
| Vertical Accuracy      | Aproximadamente 16 metros (RMS)           |
| File format      | GeoTIFF                        |
| Altitude Unit       | Metros sobre el nivel del mar (msnm)      |
| Coordinate system  | WGS 84                                     |
| Data version        | SRTM-1 (30 metros)    |
| Date of Acquisition    | 2014-09-23 |
| Data Provider      | NASA, USGS                                 |
| Download URL         | https://earthexplorer.usgs.gov/|

The Slope, Aspect, and general curvature were obtained from de DEM using the open software SAGA GIS (https://saga-gis.sourceforge.io/en/index.html).
