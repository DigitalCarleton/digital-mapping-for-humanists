---
description: >-
  Written by Rebecca Ciota and Ellen Joyce. Edited by Alan Zheng. Reviewed by
  Austin Mason and Aaron Young.
---

# Neatline for Humanistic Mapping

## **Introduction**‌

According to the [Neatline](https://neatline.org/) website:

“**Neatline allows scholars, students, and curators to tell stories with maps and timelines.** As a suite of add-on tools for [Omeka](http://omeka.org/), it opens new possibilities for hand-crafted, interactive spatial and temporal interpretation.”

Neatline has a rather steep learning curve, so it is probably most useful for those who are already using Omeka to create online exhibits and want to integrate maps into those 0pprojects. It involves manually drawing points, lines, and areas on a base layer, rather than importing spreadsheet data; those become “records,” which can be linked to Omeka items \(which can have rich metadata\).

{% hint style="danger" %}
**This Recipe is an Advanced Level Recipe.** 

**Proceed with caution**
{% endhint %}

## **Ingredients**

**Omeka Classic** – [Omeka](https://omeka.org/) is an open-source web-publishing software, specifically designed for library, museum, archives, and other scholarly collections. [Omeka Classic](https://omeka.org/classic/) is the original version of Omeka. The development community has moved to Omeka S, but Omeka Classic is still valuable for individual projects.

**‌Access to a LAMP server** that can host Omeka Installations \(either through your institution or by renting server space; we recommend Reclaim Hosting if you decide to host it externally, but contact your IT and library staff for their recommendations\).

**Neatline plugin for Omeka** – [Neatline](https://omeka.org/classic/plugins/Neatline/) is a framework for creating interactive versions of visual materials such as maps, paintings, and photographs. Neatline was built as a plugin for Omeka Classic. Find the documentation [here](http://docs.neatline.org/).

**Web browser**

**Login information** for your Omeka site

**Administrator privileges** on the Omeka site \(you want to be at least an Administrator, though Super Users are the only ones who can make exhibits private or public. \(YOU CAN GET THIS SIMPLY BY BEING INVITED TO JOIN SOMEONE ELSE’S OMEKA INSTALLATION‌, in which case you can skip to section 2. Create an Exhibit, below.

## **How to do it**

‌Once you have logged into your Omeka installation, you will need to install the Omeka Neatline plugin.

1. **Install Plugins for Neatline mapping within Omeka**

We recommend using [**Escher**](https://github.com/Daniel-KM/Omeka-plugin-Escher), an Omeka plugin, to help you install Neatline and its related plugins; otherwise you will need to install them in the plugin section of your server’s file manager.

* Neatline
* Neatline Widget SIMILE Timeline
* Neatline Widget ~ Waypoints

Optionally, you might also install and select the NeatLight theme \(download this and then select it using the “Appearance” menu in your Omeka installation\).

Once you have uploaded your plugins \(which is really easy if you use the Escher plugin for Omeka\), go to the Plugin menu in Omeka to finish installing and configuring the plugins \(the install button is the green button\).

2. **Create an Exhibit.** Click on the Neatline link which should have appeared in the left hand navigation menu.

* You may be asked to provide a Google API in order to use Google base layers for your map--you can go to Google, give them your credit card information, and get that API, for which you will probably never actually be charged, or you can ignore this step for now.

You will be asked to complete the following fields \(you can come back to edit your settings later\):

* Provide a Title and a URL-slug \(both required\).

A URL-slug is the part of a web address that comes at the very end of the URL, and identifies a specific page or post. Try to keep your 'slug' short \(3-5 words\) and descriptive, including key word if possible.

* At this time you may write a narrative description of your exhibit \(or you can add it later\)
* In the Widgets input, add SIMILE Timeline and/or Waypoints if you would like a timeline to appear at the base of the map and/or an organized list of your map data to appear to the right.
* Enable Spatial Layers: you can choose the layers you would like to use.

If you have a Google API, you can use the Google map layers. Otherwise, OpenStreetMap and the Stamen options \(Toner, Watercolor, Terrain\) are available. Choose one of those maps as the default layer. \(You need to give Google your credit card but you probably won’t be charged...talk to your IT people\).

* Required: Select a default Spatial Layer that will be the basemap for your exhibit until/unless you change it.
* Neatline gives you options to further customize the base layer. You can ignore those for now unless you know that you plan to use an image or an imported map for your base layer.
  * Guess what? You don’t need to use a map with Omeka. You can use an image for your base layer and build an exhibit with that. You might want to use an historic map, for example\).
  * In the exhibit settings, under Default Spatial Layer, pick “None.”
  * You have to make this decision at the outset, otherwise you’ll only be able to view maps.
* Check the box to make your site public.
* **Click Save** Save OFTEN with Omeka and Neatline--they do NOT save automatically.

**3. Working with your exhibit**

Your exhibit will now appear in a list \(when you have more than one\) when you click on the Neatline tab in the left sidebar. Click on the title of the exhibit to edit the map exhibit itself \(you may also return to exhibit settings, etc. as necessary\)

When you open the map, you will find it centered on the ocean south of West Africa. Navigate to where you would like to work on the map and zoom in to the extent you need for your project.

**Records** are the key ingredient for customizing your map. They are linked to places you would like to show on a map; they can be points \(one specific place\), lines \(a trajectory or connection\), or polygons \(a region\).

* Create a record by selecting New Record.
* Give your record a Title and fill in any other fields you like.
* Use the Map and Style tabs to **place points, draw lines and polygons** and to change their appearance. Playing around with these attributes is the best way to learn about them.
* Once you have placed a point, line, or shape on the map, you should be able to see a brief pop-up menu with its title when you mouse over it, and to see more information \(including its metadata if it is linked to an Omeka item\) if you click on it.

**Remember to SAVE every time you move from one menu to the next!** \(Neatline does NOT save automatically\).

**4. Connecting to Omeka data:**

 To do this, you need a working knowledge of Omeka’s exhibit building software, which is beyond the scope of this recipe. A good starting place is the Omeka Classic user manual: [https://omeka.org/classic/docs/](https://omeka.org/classic/docs/), though you may want to seek out further assistance.

* Records can also link to Omeka items, if your site has items.
* Items are a great way of giving your places metadata and associated date. For example, you can connect a picture of a Greek vase to Greece or to the place it was excavated.
* If there is an item, you can hover over the place and get the title of the record. If you click the place, you can see the item, including an image, if that is part of the item’s record.

## **How it works**

\[Working on this section\]

A detailed explanation of what happened in the previous section, so we are not perpetuating technology "black boxes" but helping people understand how to take control.

This section can include code snippets of CSS, JavaScript, Python, etc.

as appropriate

## **Further Resources**

‌\[Working on this\]

This section can be used to give additional information to make the reader more knowledgeable about specific aspects of the recipe, or provide helpful links to other useful information.

