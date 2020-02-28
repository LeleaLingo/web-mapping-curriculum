<h2>Data prep and analysis</h2>
<b> Find at least two web mapping examples that allow for user analysis. For each example provide: 1) a link to the web map and 2) a description of the user analysis</b><br>
1. https://www.zillow.com/homes/for_rent/ (the "draw" feature in the top right of the map).  This web map has a feature which allows the user to draw a polygon around the area they are interested in, and once selected it shows the available properties in that area (that meet the other search criteria controlled by the user).<br>
2. https://www.mapmyrun.com/routes/create/ (sorry, you have to log in to access it!). This web map allows the user to plan a run route, either by selecting a start and midpoint and having the map generate a return route, or by clicking waypoints to complete the whole route. The user can define if they would like to take elevation and/or distance into account, and the data the user has requested will be displayed.<br>
<b>Give an example of static data you might include on a web map. How is your example different from dynamic data?</b>
Static data would be a topographic base layer on a webmap showing trails or geocaches or some other data. It is static because the user can see the information but not interact with it, whereas the dynamic trails or geocache locations are things that could be clicked on to provide other information, etc.
<br>
<b>Under what circumstances might you want to do some data prep in desktop GIS before incorporating data into your web map? Give an example of the type of data that might apply here. </b>
Most commonly, you would want to do data prep in GIS with data that you intend to display in a static form in your web map. GIS can also help manage data that you will use dynamically, for example if you had obtained state-wide data and are making a county-sized web map, you could use GIS to clip the data to only the data geographically associated with the county to help keep file size down. An example of the type of data in this secon scenario would be forest fire data. CalFire provides data showcasing all forest fire data across the state. If you were creating a webmap to show forest fire threats within Alameda County, you could prep the data in GIS by clipping Alameda County data only, and omit the rest of the state's data.
<br>
<b>What are some data characteristics that can impact rendering speed? How might you address these issues?</b>
Rendering speed is greatly impacted by the amount of information needing to be processed on the user end. Vector tiles already containing static data can help to reduce the amount of information that the user's computer needs to render and speeds up rendering for dynamic data.
<br>
<b>What is turf.js? Give an example of how you could apply a turf operation to a web map.</b>
Turf.js is a geojson compatible geospatial analysis system which allows for various types of user analysis. An example of the turf operation is to measure a distance on the map (related to the MapMyRun answer above).
<br>
<h2>Inline writing prompts</h2>
<b>Describe where the centroids variable comes from. How is it possible for you to reference this variable when you didn't declare it?</b>
The centroids variable comes from the centroids.js JavaScript file I created in the same folder as the homework file. I am able to reference it because I linked it to my webpage as a source in the HTML head.
<br>
<b>Why might you want to create the 'centroids-selected' layer after you've created the 'centroids' layer?</b>
The selected centroid can only be executed when a centroid is selected, so you have to actually create the centroid layer for the computer to render BEFORE the user can select one (and then trigger the centroids-selected programming).
<br>
<b>Should you set the marker's lngLat and add it to the map? Why or why not?</b>
No, you should not, because the marker's lngLat depends on where the user clicks!
<br>
<b>How did you know which arguments to pass to the pip() function?</b>
If you search pip in the code provided, it is defined lower down in the code and it defines the parameters you need to use.
