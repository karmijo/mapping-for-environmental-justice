# Technical Scope

## 1. Web mapping solution
### Carto.js version 4.2.0
  - Our shapefile data is uploaded to Carto as a public dataset named "mej_colorado_final" (supports advanced PostGIS capabilities as a geospatial database) and is synced with our map
  - Custom web interface created using mainly the Carto.js v4.2.0 library and the Leaflet.js library

## 2. Features

1. **Map layers**
  - baselayer from Carto Voyager without labels, label layer from Stamen designs (http://maps.stamen.com/terrain-labels/#12/37.7706/-122.3782)
  - choropleth styling based on the colorado_final dataset 
2. **Styling map colors**
  - using Turbo-Carto CSS (https://carto.com/developers/styling/turbocarto/) to style choropleth map
3. **Data dictionary**
  - key: rank column title in dataset
  - value: JSON object with the categories: official display name, score column name, parent indicator (ex. population characteristics or pollution burden), choropleth colors, number of quantiles for ramp, and indicator descriptions for the popup
4. **Home button within zoom bar**
 - using tutorial: http://jsfiddle.net/pqfche83/1/
5. **Geocoder/search bar**
 - using Leaflet plugin from https://github.com/perliedman/leaflet-control-geocoder
6. **Polygon highlight when clicked**
 - using Carto SQL API https://carto.com/developers/sql-api/guides/making-calls/
7. **Style dropdown menu**
 - using Bootstrap select to style dropdown: https://developer.snapappointments.com/bootstrap-select/examples/
8. **Change map coloring**
 - using setContent() from carto.style.CartoCSS
9. **Popup**
 - Leaflet popup: https://leafletjs.com/reference-1.6.0.html#popup
 - HTML table: https://www.w3schools.com/html/html_tables.asp
 - Bootstrap Collapse to make table responsive: https://getbootstrap.com/docs/4.0/components/collapse/
 - HTML dataset to save data corresponding to each row for "2nd page" of popup: https://www.youtube.com/watch?v=6BdKUO2QbA0
10. **Font awesome icons**
 - https://fontawesome.com/v4.7.0/icons/
11. **Change positions of features based on screensize**
 - using CSS @media https://www.w3schools.com/cssref/css3_pr_mediaquery.asp
