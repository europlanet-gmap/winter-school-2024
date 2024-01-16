# 2024 GMAP Winter School - Ganymede basemap data sources

Raster data from USGS Astrogeology, see references below, derived from:

## Original acess URL

https://astrogeology.usgs.gov/search/map/Ganymede/Voyager-Galileo/Ganymede_Voyager_GalileoSSI_global_mosaic_1km

## Data package availability 

https://zenodo.org/doi/10.5281/zenodo.10515746

## Coordinate Reference Systme (CRS)

Please note that the CRS below might not be following IAU, see also original source link and [CRS](https://github.com/europlanet-gmap/winter-school-2024/tree/main/crs)

* Longitude: 0-360
* Positive East (as common on Dekstop GIS)

### Proj4 CRS (same as source:

```
+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=180 +x_0=0 +y_0=0 +R=2632344.9707 +units=m +no_defs
```
### WKT CRS

```
PROJCRS["SimpleCylindrical Ganymede",
    BASEGEOGCRS["GCS_Ganymede",
        DATUM["D_Ganymede",
            ELLIPSOID["Ganymede",2632344.9707,0,
                LENGTHUNIT["metre",1,
                    ID["EPSG",9001]]]],
        PRIMEM["Reference_Meridian",0,
            ANGLEUNIT["degree",0.0174532925199433,
                ID["EPSG",9122]]]],
    CONVERSION["Equidistant Cylindrical",
        METHOD["Equidistant Cylindrical",
            ID["EPSG",1028]],
        PARAMETER["Latitude of 1st standard parallel",0,
            ANGLEUNIT["degree",0.0174532925199433],
            ID["EPSG",8823]],
        PARAMETER["Longitude of natural origin",180,
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

Batson, R. M. (1984). Voyager 1 and 2 Atlas of Six Saturnian Satellites (NASA-SP-474). Washington, DC: National Aeronautics and Space Administration (NASA). https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/19840027171.pdf

Batson, R. M. (1987). Digital cartography of the planets—New methods, its status, and its future. Photogrammetric Engineering and Remote Sensing, 53(9), 1211–1218.

Becker, T. L., Archinal, B. A., Colvin, T., Davies, M., Gitlin, A., Kirk, R. L., & Weller, L. (2001). Final digital global maps of Ganymede, Europa, and Callisto. Paper presented at the 32nd Lunar and Planetary Science Conference, Lunar and Planetary Institute, Houston, TX. https://www.lpi.usra.edu/meetings/lpsc2001/pdf/2009.pdf

Gaddis, L. R., Anderson, J., Becker, K., Becker, T., Cook, D., Edwards, K., Eliason, E., et al. (1997). An overview of the Integrated Software for Imaging Spectrometers (ISIS). Paper presented at the 28th Lunar and Planetary Science Conference, Lunar and Planetary Institute, Houston, TX. https://www.lpi.usra.edu/meetings/lpsc97/pdf/1226.pdf

Greely, R., & Batson, R. (2007). Planetary Mapping. (ISBN 0-521-30774-0). New York, NY: Cambridge University Press.

Kirk, R. L., Thompson, K. T., Becker, T. L., & Lee, E. M. (2000). Photometric modeling for planetary cartography. Paper presented at the 31st Lunar and Planetary Science Conference, Lunar and Planetary Institute, Houston, TX. https://www.lpi.usra.edu/meetings/lpsc2000/pdf/2025.pdf

McEwen, A. S. (1991). Photometric functions for photoclinometry and other applications. Icarus, 92, 298–311. https://doi.org/10.1016/0019-1035(91)90053-V
