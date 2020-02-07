<!DOCTYPE html>
<html>

<head>
  <title>Quick Start - Mapbox GL JS</title>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="shortcut icon" type="image/x-icon" href="docs/images/favicon.ico" />
  <!-- Add a `link` tag for Mapbox GL JS's CSS -->
  <link href='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.css' rel='stylesheet' />
  <!-- Add a `script` tag for Mapbox GL JS's JavaScript -->
  <script src='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.js'></script>
  <!-- Set the map's width: 800px and height: 600px in a `style` tag -->
  <style type="text/css">
    #mapId {
      width: 800px;
      height: 600px;
    }

  </style>
</head>

<body>
  <!-- Create a div to house the map -->
  <style>
    #fly {
    display: block;
    position: relative;
    margin: 0px auto;
    width: 50%;
    height: 40px;
    padding: 10px;
    border: none;
    border-radius: 3px;
    font-size: 12px;
    text-align: center;
    color: #fff;
    background: #ee8a65;
    }
    </style>
    <div id="map"></div>
    <br />
    <button id="fly">Click Here</button>  
  
  <div id="mapId"></div>
  <script>
    // Set your Mapbox access token
    mapboxgl.accessToken = "pk.eyJ1IjoibGVsZWFsaW5nbyIsImEiOiJjazU3YjhmeWIwYzFmM3BwNzRtZncxZ2hyIn0.rNu-6Hs3U5-C1B1kL7YRJw";

    /* Create a variable called "map" and use it to store a new mapbox gl map.
    * Set your map's center to [-122.467, 37.798] and zoom to 13. 
    * Set the style URL to "mapbox://styles/mapbox/light-v10" 
    * See the Mapbox GL JS API reference for more info: https://docs.mapbox.com/mapbox-gl-js/api/ 
    */
    var map = new mapboxgl.Map({ 
        container: "mapId",
        center: [-122.467, 37.798],
        zoom: 13,
        style: "mapbox://styles/mapbox/light-v10"
    })

    /* Create a variable called "popup" to store a new Popup instance (ref: https://docs.mapbox.com/mapbox-gl-js/api/#popup). 
     * and set its HTML content to:
     * "<b>The Presidio.</b><br /> Explore to find a drinking fountain!"
     * set lng lat to the center of the map
     */
    var popup = new mapboxgl.Popup({ closeOnClick: false})
    .setHTML('<b>The Presidio.</b><br /> Explore to find a drinking fountain!');

    /* Create a variable called "marker," 
     * add to it a new Marker (ref: https://docs.mapbox.com/mapbox-gl-js/api/#marker),
     * set its Lng, Lat to [-122.4700, 37.8011],
     * set its popup to the popup variable you created earlier,
     * and add it to the map.
     */
    var marker = new mapboxgl.Marker()
    .setLngLat([-122.4700, 37.8011])
    .setPopup(popup)
    .addTo(map);
    
 document.getElementById('fly').addEventListener('click', function() {
   map.flyTo({
     center: [-118.34, 46.06],
    essential: true
  });
});



  </script>
</body>

</html>