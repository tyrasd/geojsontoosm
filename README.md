geojsontoosm
============

Converts [GeoJSON](http://www.geojson.org/) to [OSM](http://openstreetmap.org) [data](http://wiki.openstreetmap.org/wiki/OSM_XML).

Usage
-----

* as a **command line tool**:
  
        $ npm install -g geojsontoosm
        $ geojsontoosm file.geojson > file.osm
  
* as a **nodejs library**:
  
        $ npm install geojsontoosm
  
        var geojsontoosm = require('geojsontoosm');
        geojsontoosm(geojson_data);

* included **a browser**:
        Install browserify globally, probably need sudo:
        $ npm install -g browserify

        create the js file for the browser: 
        $ browserify node_modules/geojsontoosm/index.js -d --s geos  > dist/pizza.js

        Now include pizza in your project

        <script src="dist/pizza.js" charset="utf-8"></script>

        And you can call with geos() in your project:
        var xml = geos(JSON.parse(json));
