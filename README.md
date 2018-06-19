# apigoogle-maps


<!doctype html>
    <html>
        <head>
            <title>map</title>
            <style>
                *{
                    margin:0;
                    padding:0;
                }
                #map{
                    height:500px;
                    width:100%;
                }
            </style>
        </head>
        
        <body>
            <div id="map"></div>
            
            <script>
            function initMap(){
                var location = {lat: 30.5595,lng: 22.9375};
                var map = new google.maps.Map(document.getElementById("map"),{
                    zoom: 4,
                    center: location
                });
                var marker = new google.maps.Marker({
                    position: location,
                    map: map
                });
            }
            </script>
            <script async defer src="https://maps.googleapis.com/maps/api/js?key=AIzaSyCwAGsx5ISxflSvFoFlvPXvxtoFFDH0SMY&callback=initMap"></script>
        </body>
</html>
