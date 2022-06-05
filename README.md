# Mapping_Earthquakes
# Project Overview
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

## Code
- All materials for this project are located in the [Earthquake_Challenge](https://github.com/Aigerim-Zh/Mapping_Earthquakes/tree/main/Earthquake_Challenge) folder.
    - [challenge_logic.js](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/static/js/challenge_logic.js): the code that builds the interactive map and fills it with data from an URL.
    - [index.html](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/index.html): HTML file used to build the webpage. 
    - [style.css](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/static/css/style.css): CSS file to style the page.

## Used Tools and Resources
- ```JavaScript``` and ```D3.js``` library to retrieve coordinates and magnitudes from the GeoJSON data.
- ```Leaflet``` library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data.

# Results

Using the URL for GeoJson earthquake data from the USGS website, I retrieved geographical coordinates and the magnitudes of earthquakes for the last seven days. Then I added the data to a map. 
- Pop-up marker depicts the location and magnitude. 
- Legend was added for color shading of markers according to the magnitude.

Once the basic map was created, I worked on the following deliverables.

## Deliverable 1. Add Tectonic Plate Data
To the basic map, I added tectonic plate data using ```d3.json()```, added the data using the ```geoJSON() layer```, and set the tectonic plate ```LineString``` data to stand out on the map, and added the tectonic plate data to the overlay object with the earthquake data.

![](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/Del1_GIF.gif)

## Deliverable 2. Add Major Earthquake Data
To the map in Deliverable 1, I added major earthquake data to the map using ```d3.json()```. I also added color and set the radius of the circle markers based on the magnitude of an earthquake, and add a popup marker for each earthquake that displays the magnitude and location of the earthquake using the ```GeoJSON layer```, ```geoJSON()```. 

![](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/Del2_GIF.gif)

## Deliverable 3. Add an Additional Map
Finally, I added a third map style ("Dark") to my earthquake map.

![](https://github.com/Aigerim-Zh/Mapping_Earthquakes/blob/main/Earthquake_Challenge/Del3_GIF.gif)