# google-maps

Please create the static block named 'google-maps' and paste the following code.


This is some text above google maps.
<div id="store_map" style="min-height: 300px; width: 100%;"></div>

<script type="text/javascript">
    function initialize() {
		var center_lat=34.0204989,center_lng=-118.4117325;

        var pos = new google.maps.LatLng(center_lat, center_lng);
        var mapOptions = {
            center: pos,
            panControl: true,
            zoomControl: true,
            mapTypeControl: true,
            scaleControl: true,
            streetViewControl: true,
            overviewMapControl: true,
            scrollwheel: false,
            zoom: 10
        };
        var map = new google.maps.Map(document.getElementById("store_map"), mapOptions);
    }
    google.maps.event.addDomListener(window, 'load', initialize);
</script>
