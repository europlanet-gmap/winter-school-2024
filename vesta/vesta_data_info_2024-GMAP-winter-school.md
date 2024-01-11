# 2024 GMAP Winter School - Vesta basemap data sources

TBA
## Original acess URL

TBA 
## Data package availability 

Zenodo link TBA

## Coordinate Reference Systme (CRS)

Please note that the CRS below might not be following IAU, see also original source link and [CRS](https://github.com/europlanet-gmap/winter-school-2024/tree/main/crs)

* Longitude: -180/180
* Positive East (as common on Dekstop GIS)

### Proj4 CRS (same as source:

```
+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=255000 +units=m +no_defs +type=crs
```
### WKT CRS

```
PROJCRS["unknown",
    BASEGEOGCRS["unknown",
        DATUM["unknown",
            ELLIPSOID["unknown",255000,0,
                LENGTHUNIT["metre",1,
                    ID["EPSG",9001]]]],
        PRIMEM["Reference meridian",0,
            ANGLEUNIT["degree",0.0174532925199433,
                ID["EPSG",9122]]]],
    CONVERSION["unknown",
        METHOD["Equidistant Cylindrical (Spherical)",
            ID["EPSG",1029]],
        PARAMETER["Latitude of 1st standard parallel",0,
            ANGLEUNIT["degree",0.0174532925199433],
            ID["EPSG",8823]],
        PARAMETER["Longitude of natural origin",0,
            ANGLEUNIT["degree",0.0174532925199433],
            ID["EPSG",8802]],
        PARAMETER["False easting",0,
            LENGTHUNIT["metre",1],
            ID["EPSG",8806]],
        PARAMETER["False northing",0,
            LENGTHUNIT["metre",1],
            ID["EPSG",8807]]],
    CS[Cartesian,2],
        AXIS["(E)",east,
            ORDER[1],
            LENGTHUNIT["metre",1,
                ID["EPSG",9001]]],
        AXIS["(N)",north,
            ORDER[2],
            LENGTHUNIT["metre",1,
                ID["EPSG",9001]]]]
```

## Layers 

## References
