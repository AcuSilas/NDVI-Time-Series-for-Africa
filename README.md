# NDVI-Time-Series-for-Africa
Time series animations of Earth observation imagery are captivating and engaging. In this exercise, we learn how to generate an animated GIF representing 20-year median NDVI for serial 16-day MODIS composites spanning January 1st through December 31st of the year 2020.
MODIS is a moderate resolution satellite imaging system and NDVI is a common reflectance-based vegetation index. The Earth Engine Data Catalog provides NDVI as a precalculated dataset for convenience. In the above animation, NDVI is mapped to a color gradient from tan to dark green representing low to high photosynthetic capacity (low to high vegetation cover/density/productivity). The tide-like latitudinal shift in vegetation is associated with the sun’s declination moving between 23.5° north and 23.5° south, relative to the equator, throughout the year. See Nicholson, 2019 for more information on this phenomenon. Similar seasonal patterns of vegetation productivity are found around the world at both small and large scales.

Instructions
The basic workflow is as follows:

Fetch the MODIS vegetation indices dataset and subset the NDVI band
Define region of interest and animation frame geometries
Group images from the same annual 16-day composite window using a join
Reduce the composite groups by median to produce animation frames
Define visualization parameters and convert data into RGB visualization images
Generate a URL that will produce a GIF in the browser
