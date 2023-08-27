Publishing Feature Data as OGC API Features(Challenge 1A)

- pygeoapi as basis (alternatives of course welcome)
- implement an API for publishing vector data (e.g. GeoJSON) to the API Features
  instance

To start with I have selected the Vineyards Dataset shared in the Slides. I could access it as a geojson. I have tried to publish it both as geojson and ESRI shape file. Both the alternatives work. In the providers section of my local.config I used the OGR library.

OGR stands for "OpenGIS Simple Features Reference Implementation," and it is part of the GDAL (Geospatial Data Abstraction Library) project. OGR is primarily used for reading and writing vector geospatial data formats, such as shapefiles, GeoJSON, and many others. It provides a consistent API for working with different vector data formats, making it easier for developers to handle geospatial data in their applications.

For convinience, I have dockerized the implementation. Additionally , I have used volume referenceing to add the data. Probably, for this simple implementation dockerizing is not so important. But it allows this implementation to scale up in the future.
