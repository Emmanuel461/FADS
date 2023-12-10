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
| Nombre del satélite     | Sentinel-2                                 |
| Número de banda         | Banda 1, Banda 2, ..., Banda 12             |
| Resolución espacial     | 10 metros (Banda 2, Banda 3, Banda 4)       |
|                         | 20 metros (Banda 5, Banda 6, Banda 7, Banda 8A)|
|                         | 60 metros (Banda 1, Banda 9, Banda 10, Banda 11, Banda 12)|
| Cobertura temporal      | 5 días$_{1}$                            |
| Fechas de adquisición   | From 2022-01-01 to 2022-12-31                     |
| Órbita                  | Número de la órbita                        |
| Nivel de procesamiento  | Nivel-1C, Nivel-2A$_{2}$ , Nivel-2                   |
| Plataforma de procesamiento | Copernicus Open Access Hub, etc.           |
| Sistema de coordenadas  | WGS 84                                     |
| Formato de archivo      | GeoTIFF                     |
| Proveedor de datos      | Copernicus                                 |
| URL de descarga         | https://scihub.copernicus.eu/                   |

[1]This is the process level used in this project
[2]This is the temporal resolution of the sensor, the number of images was not all in the showed period because the images with the high rate of clouds were excluded. 

The raster layers of digital elevation model (DEM) was the digital elevation-shuttle radar topography mission (SRTM): 

| Metadato                | Valor                                      |
|-------------------------|--------------------------------------------|
| Misión                  | Shuttle Radar Topography Mission (SRTM)     |
|Entity Id                | SRTM1N11W016V3                              |
| Fuente de Datos         | Radar de apertura sintética (SAR)          |
| Resolución Espacial     | Aproximadamente 30 metros (1 arco segundo)|
| Precisión Vertical      | Aproximadamente 16 metros (RMS)           |
| Formato de Archivo      | GeoTIFF                        |
| Unidad de Altitud       | Metros sobre el nivel del mar (msnm)      |
| Sistema de Coordenadas  | WGS 84                                     |
| Versión de Datos        | SRTM-1 (30 metros)    |
| Fecha de Adquisición    | 2014-09-23 |
| Proveedor de Datos      | NASA, USGS                                 |
| URL de Descarga         | https://earthexplorer.usgs.gov/|

The Slope, Aspect, and general curvature was obtained from de DEM using the open software SAGA GIS (https://saga-gis.sourceforge.io/en/index.html).
