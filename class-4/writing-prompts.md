<h2>Objects recap</h2>
<b>An object is a series of</b> keys : values. 
<br>
<b>What kinds of things can be included in an object?</b>
Objects can contain arrays, variables, strings, and other objects.
<br>
<h2>Intro to “client-side”</h2>
<b>What does client-side rendering mean in the context of web maps?</b>
It means that the data for the map is sent over the web, but the acutal graphical representation (and therefore user control and ineteraction) is rendered on the user's computer.
<br>
<b>Why is it possible for Mapbox GL JS to place labels dynamically as you interact with the map?</b>
Mapbox GL JS (and other similar systems) is client rendered, meaning that the user's computer is provided with a bunch of data and it is displaying only what the user needs or wants to see. For labels this is accomplished using collision boxes and programmed hirerarchy for the map to change labels based on zoom, angle, etc: ultimately showing the most important or most relevant labels.
<br>
<h2>Jurisdiction finder recap For the following 3 prompts, reference the working file and README.md in the jurisdiction finder explanation folder in the main class repo. </h2>
<b>Describe how feature gets to the makeFeatureLabel() function.</b>

<br>
<b>What does the getDistrictNumber() function do?</b>
It pulls the information for the district number that relates to the spot where the event (the click) happened. 
<br>
<b>Looking at the callback to map.on('click',...), what is e and why do we need it?</b>
In map.on, e is the variable assigned to the click event. We need it because it defines the event and allows future script to do what we want it to do when the click happens.
<br>
<h2>Coding</h2>
<a href="https://api.mapbox.com/styles/v1/lelealingo/ck6l7ufaq2ino1iped5sd94lg.html?fresh=true&title=view&access_token=pk.eyJ1IjoibGVsZWFsaW5nbyIsImEiOiJjazU3YjhmeWIwYzFmM3BwNzRtZncxZ2hyIn0.rNu-6Hs3U5-C1B1kL7YRJw">Check out my home!</a>
