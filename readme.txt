read me

Included the Google Maps API library script in index.html; it expects a callback of initMap function to exist.
Created function in main.js

initMap function uses navigator.geolocation.getCurrentPostion() to get the user's location. .getCurrentPosition() accepts an argument of a callback which will return a position object as an argument. Specifically, the latitude and longitude values which both live on on the coords property of the position object.

Define object userLocation that contains properties lat and lng who have their respective values.

Call initMap function.

Creates a map using constructor new google.maps.Map(<map element>, <configuration object>). Two arguments; the html element the map is attached to and an object with properties whose values configure the map's features. The properties; center (using userLocation object); zoom and scroll wheel.

Instantiates constructor to var = map.

Using the google.maps.Marker constructor to create marker. Accepts one argument, a object with properties; position, map, title. Assigns Marker instance to var = marker.