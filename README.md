This github project was inspired by Ben Balter's blog on converting Shapefiles to GeoJSON or KML.  As it turns out, there is an endless supply of geospatial data available for free.

I decided to look at my home state's gis.  The site was full of Geospatial data with meta-data, which facilitates searching.

You will need to download the gdal libraries - http://www.gdal.org/

If you have a Mac... Brew makes it really easy.

1. brew install gdal
2. ogr2ogr -f GeoJSON -t_srs crs:84 <my.geojson> <shapefile.shp>

Here's the documentation for the "ogr2ogr" http://www.gdal.org/ogr2ogr.html
