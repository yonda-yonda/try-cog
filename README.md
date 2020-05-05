# Try Cloud Optimized GeoTIFF

## Generate
```
gdal_translate in.tiff temp.tiff -co TILED=YES -co COMPRESS=DEFLATE
```
```
gdaladdo -r average temp.tiff 2 4 8 16 32 64
```
```
gdal_translate temp.tiff out.tif -co TILED=YES -co COPY_SRC_OVERVIEWS=YES
```

## View Sample
[meta.html](./sample/meta.html)

[show.html](./sample/show.html)

[show_landsat8.html](./sample/show_landsat8.html)

## Reference
[https://trac.osgeo.org/gdal/wiki/CloudOptimizedGeoTIFF#HowtogenerateitwithGDAL](https://trac.osgeo.org/gdal/wiki/CloudOptimizedGeoTIFF#HowtogenerateitwithGDAL)

[https://geotiffjs.github.io/geotiff.js/](https://geotiffjs.github.io/geotiff.js/)

[geotiff sample](https://download.osgeo.org/geotiff/samples/)

[landsat8 sample (cog)](https://landsat-pds.s3.amazonaws.com/c1/L8/139/045/LC08_L1TP_139045_20170304_20170316_01_T1/index.html)

