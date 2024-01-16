# 2024 GMAP Winter School - Venus basemap data sources

Raster data from USGS Astrogeology, see references below, derived from:

## Original acess URL

TBA 

## Data package availability 

https://zenodo.org/doi/10.5281/zenodo.10518334

## Coordinate Reference Systme (CRS)

Please note that the CRS below might not be following IAU, see also original source link and [CRS](https://github.com/europlanet-gmap/winter-school-2024/tree/main/crs)

* Longitude: -180/180
* Positive East (as common on Dekstop GIS)

### Proj4 CRS (same as source:

```
+proj=merc +lat_ts=-40 +lon_0=-90 +x_0=0 +y_0=0 +R=6051000 +units=m +no_defs +type=crs
```
### WKT CRS

```
PROJCRS["Mercator VENUS",
    BASEGEOGCRS["GCS_VENUS",
        DATUM["D_VENUS",
            ELLIPSOID["VENUS",6051000,0,
                LENGTHUNIT["metre",1,
                    ID["EPSG",9001]]]],
        PRIMEM["Reference_Meridian",0,
            ANGLEUNIT["degree",0.0174532925199433,
                ID["EPSG",9122]]]],
    CONVERSION["Mercator (variant B)",
        METHOD["Mercator (variant B)",
            ID["EPSG",9805]],
        PARAMETER["Latitude of 1st standard parallel",-40,
            ANGLEUNIT["degree",0.0174532925199433],
            ID["EPSG",8823]],
        PARAMETER["Longitude of natural origin",-90,
            ANGLEUNIT["degree",0.0174532925199433],
            ID["EPSG",8802]],
        PARAMETER["False easting",0,
            LENGTHUNIT["metre",1],
            ID["EPSG",8806]],
        PARAMETER["False northing",0,
            LENGTHUNIT["metre",1],
            ID["EPSG",8807]]],
    CS[Cartesian,2],
        AXIS["easting",east,
            ORDER[1],
            LENGTHUNIT["metre",1,
                ID["EPSG",9001]]],
        AXIS["northing",north,
            ORDER[2],
            LENGTHUNIT["metre",1,
                ID["EPSG",9001]]]]
```

## Layers 

## References

