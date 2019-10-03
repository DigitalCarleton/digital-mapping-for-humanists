# CSV File Subrecipe: Finding Latitude and Longitude for a Location; Working with locational data

Why?

This is necessary to plot locations in GIS, and to georectify historic maps

How to do it:

A\) Bing Maps Route A:

* Search the name of the entity in Bing maps search box \(or scroll and zoom to location\)
* Right click on the entity \(or location\) as it appears; coordinates should appear at bottom of a text box
* Click on “Copy” and use command Control-C to copy coordinates

B\) Google Maps Route B:

* Search the name of the entity in Google maps search box \(or scroll and zoom to location\)
* Right click on the entity \(or location\) as it appears
* Select "What's Here" in the dropdown menu
* Click on coordinates as they appear in the popup window; properly written coordinates should appear in left column

C\) Other Routes

* For topographically rich US Data, detailed coordinates can be found by scrolling, zooming, or searching: nationalmap.gov
* Programs such as AwesomeTable Geocode can be installed to facilitate finding coordinates

Importing into csv \(Comma Separated Files—such as MSExcel or Airtable or Google Sheet, etc.\), which should be recognizable across platforms, for uploading

* Copy and paste coordinates into Latitude and Longitude fields in csv file
* Make sure these coordinates are in the form of numbers and periods--not coordinates with other punctuation, direction, etc., as these will not appear in GIS, such as 47.929798, -90.371101 \(not, for example, 47°55'47.3"N 90°22'16.0"W, which will not be recognized by programs such as ARCGIS\).
* Make sure the csv file places latitude \(Y\) before longitude \(X\).

