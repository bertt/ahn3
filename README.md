# ahn3

Simple viewer for the AHN3 'bladindex'.

See https://github.com/bertt/ahn3/blob/master/ahn3.geojson

![ahn3](ahn3.png)

When clicking on the map, a popup will be shown containing a download link to raw LAZ files, for example: https://geodata.nationaalgeoregister.nl/ahn3/extract/ahn3_laz/C_50GZ2.LAZ


## source 

Source data for the GeoJSON is obtained from:

```
$ curl https://services.arcgis.com/nSZVuSZjHpEZZbRo/ArcGIS/rest/services/Kaartbladen_AHN3/FeatureServer/0/query?where=1%3D1&objectIds=&time=&geometry=&geometryType=esriGeometryEnvelope&inSR=&spatialRel=esriSpatialRelIntersects&resultType=none&distance=0.0&units=esriSRUnit_Meter&returnGeodetic=false&outFields=AHN3_LAZ&returnGeometry=true&returnCentroid=false&multipatchOption=xyFootprint&maxAllowableOffset=&geometryPrecision=&outSR=4326&datumTransformation=&applyVCSProjection=false&returnIdsOnly=false&returnUniqueIdsOnly=false&returnCountOnly=false&returnExtentOnly=false&returnDistinctValues=false&orderByFields=&groupByFieldsForStatistics=&outStatistics=&having=&resultOffset=&resultRecordCount=2000&returnZ=false&returnM=false&returnExceededLimitFeatures=true&quantizationParameters=&sqlFormat=none&f=pgeojson&token=
```

Warning: Remove the crs information otherwise basemap tiles will not show up 

