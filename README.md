[![MasterHead](https://github.com/SergioGallegoGudino/SergioGallegoGudino/blob/master/header.png)](https://github.com/SergioGallegoGudino/SergioGallegoGudino)
<!DOCTYPE html>
<html>
<head>
  <title>Change background color</title>
  <meta name="viewport" content="initial-scale=1.0, user-scalable=no" />
  <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
  <link rel="shortcut icon" href="http://cartodb.com/assets/favicon.ico" />
  <link rel="stylesheet" href="http://libs.cartocdn.com/cartodb.js/v3/3.15/themes/css/cartodb.css" />
  <script src="http://libs.cartocdn.com/cartodb.js/v3/3.15/cartodb.js"></script>

  <style>
    html, body, #map {
      background-color: #06283f;
      width:100%; 
      height:100%; 
      padding: 0; 
      margin: 0;
  </style>
</head>

<body>
  
  <div id='map'></div>
  
  <script type="text/javascript">
    function main() {

      // declare map object
      var map;
          
      //  set center and zoom level
      var options = {
        center: [40, -90], 
        zoom: 5  
      };
      
      // give options to map object
      var map = new L.Map('map', options);

      // add midnight commander basemap
      L.tileLayer('https://cartocdn_{s}.global.ssl.fastly.net/base-midnight/{z}/{x}/{y}.png').addTo(map);
      
    }
    window.onload = main;
  </script>
</body>
</html>
