<H2>Web app cartography</h2>
<b>Color plays a significant role in the visualization of map data. What are some important considerations to keep in mind when choosing the appropriate color scheme for your map?</b>
You must consider things like your audience (experts or laymen?), your data (sequential, diverging, qualitative?), and color connotations (does society already associate a color with some aspect of your data?).
<br>
<b>Why might you want to avoid using a rainbow color scheme?</b>
It can provide less information about how elements of your data relate to one another. With a rainbow color scheme it is harder for the user's brain to extrapolate quickly from your data. For example, you don't instinctively know that something colored red is greater than something colored blue, but you can (or should be able to, from a good map) make that assumption between a light blue and a dark blue. 
<br>
<b>List and describe 2-3 different thematic map types.</b>
Choropleth: Choropleths apply colors to previously designated geographic boundaries based on the quantity of things within that boundary. For example, the number of homes in a county, or the number of people in a state. Sequential colors help users to quickly understand which of the geographic areas have more/less than others. <br>
Heat map: Heat map is also geographically-based, but instead of providing data within predetermined geographic boundaries, it shows more precise geographic locations and the number of things passing over said location. Sequential colors also help here, but is different from choropleths in that it would show the user, for example, WHERE within a county population is centered instead of just the numeric populatino of the county.<br>
Cartogram: Cartograms are not geographically based in that the size of the feature is adjusted based on the data being presented. With this, a cartogram showing the population density of a state would not actually look like the state since counties with more people or more homes would be graphically represented larger than ones with fewer people. While this is interesting and informative and draws attention to the areas that are portrayed as large features, it is more difficult for the user to conceptualize and understand the rest of the data which is no longer geographically accurate or shown proportionally.
<br>
<b>What type of data is appropriately respresented by a sequential color scheme? What about a diverging color scheme?</b>
Sequential color scheme is great for things on a spectrum from 0 to 100. For example, the number of homes in a county, the number of dogs per household in an area, etc. Diverging color scheme is best used when 0 is in the middle of the data. For example, political leanings (Dem, center/independent, Republican), number of cats per household versus number of dogs per household. Here, the middle-of-the-road value would be something more neutral between two contrasting colors.
<br>
<b>Can you name any tools (either from the presentation or your web travels) that would be helpful for choosing colors?</b>
Yes, it is important to consider your data and what it is supposed to show. Once you know what the point of the map is, you can select a color scheme that will draw attention to the point you are trying to make. The most important data should be the easiest to spot when a user loads your map.
<br>
<h2>CORS and working with external data</h2>
<b>In your own words, describe why web map developers have to think about CORS.</b>
Web map developers need to consider CORS because it allows them to work around the issue of different website's "same origin" policies and times when the web map is not fully functional and only in the planning stage, so it is able to think that it is operating as it is intended to on a given server on the web, not as a draft in your file folder, for example.
<br>
<b>What is the concept of "separation of concerns?" </b>
Separation of Concerns is the idea of splitting up a program into different, distinct sections which are referenced in the end-use program or webpage. This helps with debugging, consistency across related programs or pages, and upgrades/maintenance.
