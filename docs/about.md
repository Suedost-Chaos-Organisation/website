<link rel="stylesheet" href="/assets/leaflet.css" />
<script src="/assets/leaflet.js"></script>


# About

Bei uns machen Hackende und Makende aus folgenden Spaces mit:

* [Amborg-Solzbyte](https://amborg-sulzbyte.de/) (Amberg)
* [Backspace](https://www.hackerspace-bamberg.de/) (Bamberg)
* [Binary Kitchen](https://binary-kitchen.de/) (Regensburg)
* [Bits'n'Bugs](https://erlangen.ccc.de/) (Erlangen)
* [bytewerk](https://www.bytewerk.org/) (Ingolstadt)
* [GEOLab](https://geolab.space/) (Gerolzhofen)
* [hackzogtum](https://hackzogtum-coburg.de/) (Coburg)
* [K4CG](https://k4cg.org/) (Nürnberg)
* [muCCC](https://www.muc.ccc.de/) (München)
* [Munich Maker Lab](https://munichmakerlab.de/) (München)
* [Nerd2Nerd](https://www.nerd2nerd.org/) (Würzburg)
* [Nerdberg](https://nerdberg.de/) (Nürnberg/Fürth)
* [OpenLab](https://www.openlab-augsburg.de/) (Augsburg)

<style>
    #map { height: 500px; }
</style>

 <div id="map"></div>

<script>
    var map = L.map('map');
    var CartoDB_Voyager = L.tileLayer('https://{s}.basemaps.cartocdn.com/rastertiles/voyager/{z}/{x}/{y}{r}.png', {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors &copy; <a href="https://carto.com/attributions">CARTO</a>',
        subdomains: 'abcd',
        maxZoom: 20
    }).addTo(map);

    var spaces = new L.featureGroup();
    L.marker([49.444540, 11.848280]).bindPopup("Amborg-Solzbyte").addTo(map).addTo(spaces);
    L.marker([49.901870, 10.892710]).bindPopup("Backspace").addTo(map).addTo(spaces);
    L.marker([49.009850, 12.119020]).bindPopup("Binary Kitchen").addTo(map).addTo(spaces);
    L.marker([49.579990, 10.972100]).bindPopup("Bits'n'Bugs").addTo(map).addTo(spaces);
    L.marker([48.766673, 11.425933]).bindPopup("bytewerk").addTo(map).addTo(spaces);
    L.marker([49.900403, 10.351335]).bindPopup("GEOLab").addTo(map).addTo(spaces);
    L.marker([50.263359, 10.966066]).bindPopup("hackzogtum").addTo(map).addTo(spaces);
    L.marker([49.449080, 11.080840]).bindPopup("K4CG").addTo(map).addTo(spaces);
    L.marker([48.153578, 11.560451]).bindPopup("muCCC").addTo(map).addTo(spaces);
    L.marker([48.159056, 11.547490]).bindPopup("Munich Maker Lab").addTo(map).addTo(spaces);
    L.marker([49.802064,  9.923156]).bindPopup("Nerd2Nerd").addTo(map).addTo(spaces);
    L.marker([49.470487, 11.003280]).bindPopup("Nerdberg").addTo(map).addTo(spaces);
    L.marker([48.362642, 10.902592]).bindPopup("OpenLab").addTo(map).addTo(spaces);
    map.fitBounds(spaces.getBounds());
</script>

