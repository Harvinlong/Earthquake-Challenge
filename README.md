# Mapping Earthquake
## Add Tectonic Plate Data
First, I added a second layer group variable for the tectonic plate data, and added a reference to the tectonic plate data to the overlay object to incorporate the tectonic plate data into the earthquake map.

Then, I used the d3.json() callback method to call the tectonic plate data from a GeoJSON file and pass it to the geoJSON() layer. I also styled the lines to make them stand out on all maps, and added the tectonic layer group variable I created in Step 1 to the map using the .addTo() method. Finally, I added the tectonic layer group variable to the map and closed the d3.json() callback.

After completing these steps, I started my Python server and launched the index.html file to confirm that the earthquake and tectonic plate data were displayed on the map, with all earthquakes with a magnitude greater than 4.5 visible on a third map.

![data-14-all-earthquake-data-tectonic-plate-data-on-map](https://user-images.githubusercontent.com/111480084/225198179-1511af8a-a999-47a1-90d5-387a8f188ac6.png)

## Add Major Earthquake Data
To add major earthquake data to the map, I added a layer group variable for the data, referenced it to the overlay object, and used d3.json() to call the data from the GeoJSON Summary Feed for M4.5+ Earthquakes for the past 7 days.

I then styled the data using the styleInfo() function with calls to the getColor() and getRadius() functions, and modified getColor() to use only three colors for magnitudes less than 5, greater than 5, and greater than 6.

Using the getRadius() function parameters from the previous step, I created circleMarkers for each earthquake feature on the map, styled them with styleInfo() function, and added a popup with earthquake magnitude and location.

Finally, I added the major earthquake layer group variable to the map and closed the d3.json() callback, successfully incorporating major earthquake data to the earthquake map

![data-14-earthquakes-major-earthquakes-tectonic-plate-data-on-the-map](https://user-images.githubusercontent.com/111480084/225198670-a05fe652-9394-421a-942f-913e59e04a9f.png)

## Add an Additional Map
To add a third map style to the earthquake map, I used the Mapbox styles options and added a tile layer object for the new map style to the challenge_logic.js file.

Next, I added the map variable to the base layer object and confirmed that the new map style was displayed correctly by starting the Python server and launching the index.html file.

After confirming that the new map style was correctly displayed, I verified that the earthquake map showed all three map styles and displayed both earthquake datasets and the tectonic plate data.

![data-14-three-map-style-options](https://user-images.githubusercontent.com/111480084/225198803-8f31a4da-b356-4dd3-9b7c-b81855779bfd.png)

