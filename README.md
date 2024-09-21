# mobile-tracking-app



Phone Tracker Web Application

Overview

This repository contains a simple web application built using HTML, CSS, and Leaflet.js to track phone locations on an interactive map.

HTML Structure

The HTML structure consists of:

Document Declaration


<!DOCTYPE html>
<html lang="en">


Declares the document as an HTML5 document and specifies the language as English.

Head Section


<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Phone Tracker</title>
  <link rel="stylesheet" href="(link unavailable)">
  <style>
    /* Internal CSS styles */
  </style>
</head>


Includes metadata about the document, specifies character encoding, viewport settings, and links to the Leaflet CSS library.

Body Section


<body>
  <h1>Phone Tracker</h1>
  <p>Track phone locations on an interactive map.</p>
  <form id="track-form">
    <input type="text" id="phone-number" placeholder="Enter phone number">
    <button>Track</button>
  </form>
  <div id="map"></div>
</body>


Contains the main content of the page, including a heading, paragraph, form, and map container.

Styling with CSS

The internal CSS defines the style of the page:


body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
}

h1 {
  text-align: center;
  color: #333;
}

form {
  margin: 20px;
}

#map {
  height: 500px;
  width: 100%;
}


Map Integration with Leaflet.js

The script includes the Leaflet.js library to render an interactive map:


// Initialize map
var map = L.map('map').setView([51.505, -0.09], 13);

// Add tile layer
L.tileLayer('https://{s}.(link unavailable)', {
  attribution: '&copy; <a href="(link unavailable)">OpenStreetMap</a>',
  subdomains: ['a', 'b', 'c']
}).addTo(map);


Initializes a map in the #map element, sets the initial center to London, and adds a tile layer.

Usage

1. Clone the repository.
2. Open index.html in a web browser.
3. Enter a phone number in the input field.
4. Click the "Track" button to view the location on the map.

License

This project is licensed under the MIT License.

Contributing

Contributions are welcome! Please submit pull requests or issues.
