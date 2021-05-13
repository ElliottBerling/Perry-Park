# Perry-Park
## Located at 595 Springport Ferry Rd. Perry Park KY, 40363
![logo](ElliottBerlingFinal/PPGC.jpg)
### Perry Park used to be a large slave plantation owned by the Perry family during the time of the civil war.
### It later became a golf course in the late 1960's.
### My father and his family bought the land in the 1990's and have owned and maintained it ever since.
### I have spent countless hours around this land, and it is of great importance to me.
### I hope to give this map of Perry Park along with my other maps to my Dad on Father's Day.

#### This is an overview photo of the resort.
![Overview](ElliottBerlingFinal/PPOVERVIEW.jpg)
 

## Perry Park Slide Show
# The slide show can be viewed in the link provided
# The slide show gives a 3D animation view of the first few holes on the Buckskin Golf Course.

![slideshow](ElliottBerlingFinal/Screenshot(532).png)
[Slideshow link](ElliottBerlingFinal/slideshow.html)



## Our House's Topo Map
# I created a topographic map for my Dad around our house. I know he works with topographic map everyday so I think he will enjoy this.
# Our house is indicated my the red arrow in the picture below.
# The interactive map can be seen in the link below.

![topo](ElliottBerlingFinal/mapphoto.jpg)
[map link](ElliottBerlingFinal/Mapbox.html)

<!DOCTYPE html>
<html>

<head>
  <meta charset='utf-8' />
  <title>Display a map</title>
  <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />

  <script src='https://api.mapbox.com/mapbox-gl-js/v2.2.0/mapbox-gl.js'></script>
  <link href='https://api.mapbox.com/mapbox-gl-js/v2.2.0/mapbox-gl.css' rel='stylesheet' />

  <style>
    body {
      margin: 0;
      padding: 0;
    }

    #map {
      position: absolute;
      top: 10%;
      bottom: 10%;
      width: 50%;
    }
  </style>
</head>

<body>

  <div id='map'></div>

  <script>
    // 💡💡💡 Change this to your Token --------------------
    // ------------------------------------------------
    mapboxgl.accessToken = 'pk.eyJ1IjoiZWxsaW90dC1iZXJsaW5nIiwiYSI6ImNrbzh0cndjcjB2NzIydm9hb2tkMGw4YTIifQ.FKlkT6NwV86OeAHH_0xPjw';
    // ------------------------------------------------
    // ------------------------------------------------

    var map = new mapboxgl.Map({
      container: 'map',

      // 💡💡💡 Change this to your style --------------------
      // ------------------------------------------------
      style: 'mapbox://styles/elliott-berling/ckon5wslc3jyb19pmepqjq3nm',
      // ----------------------------------------------
      // ------------------------------------------------

      // 💡💡💡 Change to your location ----------------------
      // ------------------------------------------------
      // zoom: 15.95,
      // center: [-85.009405, 38.538249],
      // pitch: 85,
      // bearing: 80
      // ------------------------------------------------
      // ----------------------------------------------

    });

    // Add geolocate control to the map.
    map.addControl(new mapboxgl.GeolocateControl({
      positionOptions: {
        enableHighAccuracy: true
      },
      trackUserLocation: true
    }));
  </script>

</body>

</html>
