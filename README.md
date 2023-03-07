# Mapping-Earthquake-with-JS-and-APIs
To add tectonic plate data to my Mapping_Earthquakes repository, I used the d3.json() function to call data from the GeoJSON/PB2002_boundaries.json data on GitHub. Once I had retrieved the tectonic plate data, I created a new layer group variable for it and added a reference to the tectonic plate data to the overlay object.

To display the tectonic plate data on my map, I added it to the geoJSON() layer and styled the lines with a color and weight that would make it stand out on all maps. Then, I added the tectonic layer group variable I created to the map using the .addTo() method, allowing me to toggle the display of the tectonic plate data on and off. Finally, I closed the d3.json() callback to complete the process.
