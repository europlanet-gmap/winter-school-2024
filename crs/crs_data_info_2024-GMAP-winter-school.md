# 2023 GMAP Winter School - CRS data sources

See also related presentatipn content at https://aprossi.eu/content/crs2024. Specific sources for each slide are also linked from there.

## Ganymede raster
Exemplary global Ganymede
maps are based on the following datasets. Each dataset is provided in difrerent CRS.

similarly to https://github.com/europlanet-gmap/winter-school-2023/blob/main/crs/crs_data_info_2023-GMAP-winter-school.md

created with proj4leaflet maps of ganymede with 

### Gegraphic (lonlat)

```
'+proj=lonlat +R=2631200 +no_defs'
```

### Equirectangular (eqc) - centered at 180
```
'+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=180 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```
### Equirectangular (eqc) - centered at 0
```
'+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```
### Cylindrical equal area (cea) - centeread at 0
```
'+proj=cea +lat_ts=0 +lon_0=0 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```
### Ortographic (eqc) - centered at 0
```
'+proj=ortho +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```
### Ortographic (eqc) - centered at 180
```
'+proj=ortho +lat_0=0 +lon_0=180 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```
### Robindson (eqc) - centered at 0
```
'+proj=robin +lon_0=0 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs'
```

plus for other demonstrations



e.g. doing a crop of a mercator with a bbox of DD, one can

```
gdalwarp -t_srs "+proj=merc +lon_0=0 +x_0=0 +y_0=0 +R=2631200 +units=m +no_defs" -te_srs "+proj=lonlat +R=2631200 +no_defs" -te -180 -80 180 80 ganymede_lonlat.tif ganymede_merc_clon0_small.tif

```

example quandrangle maps of ganymede (see ref source below)

e.g.

https://astrogeology.usgs.gov/search/map/Ganymede/Geology/Ganymede-Geologic-Map-of-the-Philus-Sulcus-Quadrangle

https://astropedia.astrogeology.usgs.gov/download/Ganymede/Geology/Ganymede-Geologic-Map-of-the-Philus-Sulcus-Quadrangle.pdf


also for vesta:

source DLR HAMO mosaic also https://astrogeology.usgs.gov/search/map/Vesta/Dawn/DLR/HAMO/Vesta_Dawn_FC_HAMO_Mosaic_Global_74ppd


```
'+proj=eqc +lat_ts=0 +lat_0=0 +lon_0=0 +x_0=0 +y_0=0 +R=255000 +units=m +no_defs'

```

## Moon vector data

Used within D3

* USGS - https://astrogeology.usgs.gov/search/map/Moon/Geology/Unified_Geologic_Map_of_the_Moon_GIS_v2
* ASU/LROC - https://wms.lroc.asu.edu/lroc/view_rdr/SHAPEFILE_LROC_GLOBAL_MARE


## Small bodies - shape models

All from PDS Small Bodies Node tool - https://sbn.psi.edu/pds/shape-models/, but one from ESA - http://comsim.esac.esa.int/rossim/SHAPE_MODEL_DRAFTS/RO-C-MULTI-5-67P-SHAPE-V3.0/DATA/SPICE_DSK/SPG_DLR/

## References

Relevant referemces for the data mentioned above:

Fortezzo, C.M., Spudis, P. D. and Harrel, S. L. (2020) Release of the Digital Unified Global Geologic Map of the Moon At 1:5,000,000- Scale. Paper presented at the 51st Lunar and Planetary Science Conference, Lunar and Planetary Institute, Houston, TX. https://www.hou.usra.edu/meetings/lpsc2020/pdf/2760.pdf

Nelson, D. M., Koeber, S. D., Daud, K., Robinson, M. S., Watters, T. R., Banks, M. E., & Williams, N. R. (2014) Mapping lunar maria extents and lobate scarps using LROC image products. In Lunar and Planetary Science Conference (Vol. 45, p. 2861).

Roatsch, T., Kersten, E., Matz, K.-D., Preusker, F., Scholten, F., Jaumann, R., Raymond, C. A., & Russell, C. T. (2012) High resolution Vesta High Altitude Mapping Orbit (HAMO) Atlas derived from Dawn framing camera images. Planetary and Space Science, 73(1), 283-286. https://doi.org/10.1016/j.pss.2012.08.021

