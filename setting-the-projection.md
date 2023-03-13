# Setting the Projection

You might have noticed that shape of DC suggested by the cherry tree dataset looks a little off. The familiar diamond shape of Washington, DC is distorted. That's because the street tree dataset we're working with was stored in EPSG 4326, a geographical coordinate system. This tells the GIS software where to place the data on the Earth, but it doesn't tell it how to translate that 3D information into a 2D drawing like we're seeing on our computer screens.

To fix this, we'll need to convert the data from EPSG 4326 to a projected coordinate system. There are thousands of projected coordinate systems to choose from, some are more appropriate for our data than others. Because we're going to use webmap tiles as the background of this map, we'll use the projection most commonly seen in webmaps, EPSG 3857, frequently referred to as Pseudo-Mercator or Web Mercator. &#x20;
