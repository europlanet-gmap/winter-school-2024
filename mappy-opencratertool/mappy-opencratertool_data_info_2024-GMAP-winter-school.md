xx# 2024 GMAP Winter School - Moon basemap data sources (for Mappy and OpenCratertool)

Raster data from USGS Astrogeology, see references below, derived from:

## Original acess URL

See Layers below.

## Data package availability 

Zenodo link TBA

## Coordinate Reference Systme (CRS)

Please note that the CRS below might not be following IAU, see also original source link and [CRS](https://github.com/europlanet-gmap/winter-school-2024/tree/main/crs)

* Longitude: 0-360
* Positive East (as common on Dekstop GIS)

### Proj4 CRS (same as source:

```
+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=1737400 +units=m +no_defs +type=crs
```
### WKT CRS

```
PROJCRS["unknown",
    BASEGEOGCRS["unknown",
        DATUM["unknown",
            ELLIPSOID["unknown",1737400,0,
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

### LROC WAC Mosaic

#### Layer access URL

https://astrogeology.usgs.gov/search/map/Moon/LRO/LROC_WAC/Lunar_LRO_LROC-WAC_Mosaic_global_100m_June2013

#### References

- Speyerer, E. J., Robinson, M. S., Denevi, B. W., & LROC Science Team (2011). Lunar Reconnaissance Orbiter Camera global morphological map of the Moon. Paper presented at the 42nd Lunar Planetary Science Conference, Lunar and Planetary Science Institute, Houston, TX. https://www.lpi.usra.edu/meetings/lpsc2011/pdf/2387.pdf

- Robinson, M. S., Brylow, S. M., Humm, D., Lawrence, S. J., Thomas, P. C., Denevi, B. W., Bowman-Cisneros, E., et al. (2010). Lunar Reconnaissance Orbiter Camera (LROC) instrument overview. Space Science Review, 150(1), 81–124. https://doi.org/10.1007/s11214-010-9634-2

- Wagner, R. V., Speyerer, E. J., Robinson, M. S., & LROC Team (2015). New Mosaicked Data Products from the LROC Team. Paper presented at the 46th Lunar and Planetary Science Conference, Lunar and Planetary Institute, Houston, TX. https://www.hou.usra.edu/meetings/lpsc2015/pdf/1473.pdf Eposter: http://www.lpi.usra.edu/meetings/lpsc2015/eposter/1473.pdf

- Sato, H., Robinson, M. S., Hapke, B., Denevi, B. W., & Boyd, A. K. (2104). Resolved Hapke parameter maps of the Moon. Journal of Geophysical Research: Planets, 119, 1775-1805. https://doi.org/10.1002/2013JE004580

### LOLA and Kaguya TC merged DEM 60N-60S 59m/pixel

#### Layer access URL

https://astrogeology.usgs.gov/search/map/Moon/LRO/LOLA/Lunar_LRO_LOLAKaguya_DEMmerge_60N60S_512ppd

#### References

- Barker, M. K., Mazarico, E., Neumann, G. A., Zuber, M. T., Haruyama, J., & Smith, D. E. (2016). A new lunar digital elevation model from the Lunar Orbiter Laser Altimeter and SELENE Terrain Camera. Icarus, 273, 346–355. https://doi.org/10.1016/j.icarus.2015.07.039

- Haruyama, J., Matsunaga, T., Ohtake, M., Morota, T., Honda, C., Yokota, Y., Torii, M., Ogawa, Y., & LISM Working Group (2008). Global lunar-surface mapping experiment using the Lunar Imager/Spectrometer on SELENE. Earth Planets Space, 60, 243-255. https://doi.org/10.1186/BF03352788

### Clementine UVVIS Warped Color Ratio Mosaic 200m v1

#### Layer access URL

https://planetarymaps.usgs.gov/mosaic/Lunar_Clementine_UVVIS_Warp_ClrRatio_Global_200m.tif

#### References

- Lucey, P. G., Blewett, D. T., Taylor, G. J., & Hawke, B. R. (2000). Imaging of lunar surface maturity. Journal of Geophysical Research: Planets, 105(E8). https://doi.org/10.1029/1999JE001110

- McEwen, A. S., & Robinson, M. S. (1997). Mapping of the Moon by Clementine. Advances in Space Research, 19(10), 1523-1533. https://doi.org/10.1016/S0273-1177(97)00365-7

- Nozette, S., Rustan, P., Pleasance, L. P., Kordas, J. F., Lewis, I. T., Park, H. S., Priest, R. E., et al. (1994). The Clementine Mission to the Moon: Scientific Overview. Science, 266(5192), 1835-1839. https://www.doi.org/10.1126/science.266.5192.1835
