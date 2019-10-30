---
description: >-
  Written by Louis K Epstein. Edited by Alan Zheng. Reviewed by Austin Mason and
  Aaron Young
---

# Many Stub Ideas with some instructions

## **ArcGIS Tricks**

* When uploading a layer, fill out the metadata fields
* Making Maps Public: The layer that you upload needs to be made public \(Share→ Everyone\), right when you upload it. Then the map also needs to be made public once you’re done \(again, Share→ Everyone\).
* Postal Codes will initially be read as an Integer. Change it to read as a String.
* Configuring Pop-Ups: Click on the three blue dots to the far right under the title of your layer. Then scroll down to “configure pop-up.” This will allow you to edit the info window.

## ![](../.gitbook/assets/0%20%282%29.png)

* Within the “Configure pop-ups” Menu, selecting “Configure attributes” will allow you to select which information you want to see \( ex. You can exclude latitude/longitude\), and arrange each category in the order you like. You can also edit how each category title will appear.

### IMAGES:

* Make sure that you’ve entered an image URL in the database for each venue/event that you want to map. These can be URLs from external sites, or from a PUBLICLY shared Google Photos album. \(Get the image urls from the public view of the album- log out of gmail to make sure it works\).
* Export and upload the CSV as normal.
* Under the “Configure Pop-ups” menu, scroll down to “Pop-Up Media.” Click Add Media→ Image.
* In the window that appears, the title and caption are optional and up to you. For URL and Link, click the small plus sign to the right of each box and scroll down to select “Image {ImageLink}.” This connects the info window to the Image Link column of the database, where you pasted the URL.
* Hit OK to save within the window, and then make sure to click OK again in the “Configure Pop-Up” window to save your changes.
* If you want to change the image title, etc., click the small gear icon under the Pop-Up Media section to make edits. Note that unless there’s a separate column for it in the database, any words that you write will be the same across all points on the map \(for example, they will all have the same title/caption if you choose to include one\).
* The images always appear at the bottom of the info window, and \(as far as we know?\) there’s no way to change that. To see the images in a larger view, right click and open them in a new tab.

### YOUTUBE CLIPS:

* In a “Media” field, include the following code around a Youtube link \(in bold below; doesn’t need to be bolded in the spreadsheet\):
  * &lt;iframe width="280" height="157.5" src="**https://www.youtube.com/embed/RmfdXF7zWlI**" frameborder="0" allowfullscreen&gt;&lt;/iframe&gt;

```text
<iframe width="280" height="157.5" 
src="https://www.youtube.com/embed/RmfdXF7zWlI" frameborder="0" allowfullscreen></iframe>
```

* Creating hosted feature layers from Google sheets:
  * This is useful to do so that you can search and filter by a given layer. If you are simply wanting to create a map layer that automatically updates from google sheets, but does not need to be searched or filtered, you can do so by following the instructions for [How-To: Google Docs in ArcGIS Online Maps](https://www.youtube.com/watch?v=jG37zPui1r4)
  * To create a hosted feature layer, go to your arcgis online “content” page and clicking “add item” –&gt; “from cloud drive” \(Make sure to allow pop-ups so that you can access your google drive account\)
  * Next, go to the drop-down menu that says “CSV” and select your desired file type, presumably a google sheet, search for and select your desired file, and follow the instructions from there.
  * Once this feature layer is created, you can add it to a map by going to add –&gt; search for layers.
  * NB: A hosted feature layer does NOT automatically sync with google sheets, and a map using a hosted feature layer does NOT automatically sync with changes made to that hosted feature layer. In order to sync a map with a hosted layer automatically, you can click “more options” \(the blue ellipsis\) on the layer from within the map that you’ve added it to and then adjust the refresh interval.
  * In order to sync a google sheet based hosted layer with its original sheet, go to the hosted layer and click “update data” –&gt; “overwrite entire layer”. Once this is done, the map will refresh automatically with the new data if it has been set to do so. \(See point above\)
* Searching feature layers:
  * First, make your feature layer that you want to search within a [hosted feature layer](https://doc.arcgis.com/en/arcgis-online/manage-data/publish-features.htm)
  * Then, in the web-app editor, go to widgets, hover over the search widget, and click the pencil icon to configure this widget.
  * Click “add search source” and select your new hosted feature layer.
  * Select your desired search fields \(which field you want the users to be able to search\) and your desired display field \(the field which will be displayed as possible options when the user is selecting a result to display from their search\) Adjust any other options as desired.
* Filtering features:
  * There is a widget for this. Like searching, the filterable layers must be hosted feature layers.
  * You can create one’s own filters that the user can turn on and off by editing the widget. You can also allow the user to create custom filters \(turned off by default\) by checking the box in the lower left. \(At least it is in the lower left as of 1/22/19\)
  * NB: Though allowing users to create custom filters may sometimes be what you want, the custom filter menu is quite confusing and not user friendly, particularly for those who might not be as familiar with database searching and filtering menus as you are after all of your research. Therefore, you might want to consider trying to exhaustively and explicitly list any filters that might be interesting, rather than leaving the user to try and figure it out. \(Also note that this is simply for filtering within layers. If one wants to give users the option to turn layers on or off, there is another widget for that that is much easier to use called “layer list”\)
* Creating time aware feature layers to use with a time slider:
  * First, you must make sure that the desired layer has all of the dates in the **same** format - ambiguity and inconsistency is not allowed.
    * To deal with ambiguity in dates, [see the relevant recipe](https://docs.google.com/document/d/1bPy9dD6_x6Fb_UKTcmUzfVZ2o7JrjQOReDj2i176tME/edit?usp=sharing).
  * Then, create a hosted layer and make it time-enabled.
    * [https://doc.arcgis.com/en/arcgis-online/create-maps/configure-time.htm](https://doc.arcgis.com/en/arcgis-online/create-maps/configure-time.htm)
    * I have been having issues making layers that are created from a google sheet time-enabled - I keep getting strange error messages. If this is the case for you too, then you will have to download the data as a CSV and re-upload it to create the hosted feature layer that is time-enableable
  * The time slider should show up automatically on the map viewer. To add it to the web-app, simply add the time-slider widget.
* TODO:
  * Spidering/dealing with overlapping points

