<h1> Writing Prompts</h1>
<b>What is the difference between raster and vector data?</b>
Raster data are 'pictures' or 'tiles' that can show maps or pictures taken from satelites (i.e. as a base layer). These are rendered and stored ahead of time and cannot be changed on the fly or interacted with. Vector data consists of points, lines, and polygons. It can be layered, filtered, and updated as the user needs. Vector data is also often interactive in that there is additional data stored about a particular point, line, or polygon.
<br>
<b>Why do "slippery maps" exist?</b>
Slippery maps exist to make it faster for the user to pan around. It means the website pre-loads tiles around the displayed tiles so that when the user pans in any direction, the information is already loaded.
<br>
<b>Why would you want to install a dedicated text editor?</b>
Dedicated text editors are 'smart' in that they may change colors for different kinds of code, can predict the end to codes (i.e. automatically insert </ > for a given command), and are otherwise designed to make coding easier.
<br>
<b>What is Leaflet?</b>
Leaflet is an open source JavaScript library. It can be referenced while coding as a 'shortcut' to having an already established, coded map that you can just update to personalize it and make it fit the project at hand. It provides a clear framework of code to be ammended.
<br>
<b>How has web map rendering changed over the years?</b>
Map rendering has changed significantly, but the bottom line is the map tiles originally were rendered, saved, and stored on a host that each computer would ping for individual map tiles. Changes to map data required a new set of tiles to be rendered, re-saved, etc. It was cumbersom and did not allow for personalization and easy editing. Over the years map rendering has changed into predominatnly vector data which is stored on hosts and individual computers do the rendering. The change has made map rendering much faster and more user-friendly.
<br>
<b>What is the basemap-overlay paradigm and how are GL maps different?</b>
The basemap-overlay paradigm is a basemap made of tiles with data layers displayed over top of them. This is essentially how ArcGIS basemaps work. GL maps contain much of the same data as would be displayed, but instead it is all layer-based. This allows for easier customization and editing. GL maps are becoming more frequently used.
<br>
<b>What kind of interactions do you see? Why might you use each of those interactions?</b>
One of the MapBox user interactions is 'Disable map rotation'. This locks the map in 'North Up' and can be used if having geographical awareness of the area being displayed is especially important. For example, if a map you are building does not have roads or other cues to help the user keep awareness of the map orientation (i.e. maping things offshore or in a forest or desert), you can lock the rotation so it is always oriented the same way. Another handy interaction is 'Filter symbols by text input' which allows the user to search a layer of data with a textbox. This is helpful if there is alot of information in a layer, and the user can apply the filter to only see the information applicable to what they are interested in. 
<br>
<h1>Exercises</h1>
<a href="https://api.mapbox.com/styles/v1/lelealingo/ck61hzdhi04zl1inusko7lt6k.html?fresh=true&title=view&access_token=pk.eyJ1IjoibGVsZWFsaW5nbyIsImEiOiJjazU3YjhmeWIwYzFmM3BwNzRtZncxZ2hyIn0.rNu-6Hs3U5-C1B1kL7YRJw"> Check out my cool Choropleth! </a>
<br>
