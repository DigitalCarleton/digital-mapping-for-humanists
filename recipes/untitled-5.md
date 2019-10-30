---
description: >-
  Written by Mark Thorne. Edited by Alan Zheng. Reviewed by Austin Mason and
  Aaron Young.
---

# Map locations from a text using Recogito

## **Introduction**

If you want to generate a map of place names mentioned in a text, [Recogito](https://recogito.pelagios.org/) \([https://recogito.pelagios.org/](https://recogito.pelagios.org/)\) is a useful web-based tool that is free to use. This data can then be exported in CSV, RDF, or GeoJSON formats \(plus a few others\) for uploading into other GIS programs for further work or analysis.

{% hint style="danger" %}
WARNING: Please note that this tool is designed primarily for identifying cities, islands, and regions. It is not able to map roads, individual buildings, street addresses, etc. The reason for this is that the gazetteer information upon which this tool relies does not contain that kind of information.
{% endhint %}

## **Ingredients**

You will need:

* A Recogito account \(it’s free!\)
* Your chosen text in .txt or .xml format \(UTF-8 format\)

Recogito only generates a map of places you specifically annotate; to manipulate the generated mapping data further, you will need access to a GIS or other mapping program.

WARNING: If you are exporting a .txt file from MS Word or similar program, make sure to encode it as UTF-8 format rather than Windows standard.

## **How to do it**

Head to [https://recogito.pelagios.org/](https://recogito.pelagios.org/) and:

1 - Create an account or sign in

2 - Click “New” at the upper left under your account name to upload a text

3 - Double-click on your text to open it for annotations

{% hint style="success" %}
**Where can I find the texts?**

[Project Gutenberg](https://www.gutenberg.org/) is a very useful resource if you are considering mapping places from historical literature. You can also contact your institution's librarians and archive researchers to help you obtain source materials to analyze.

It is also very possible that you already have found your texts and are just looking for a way to map it. 
{% endhint %}

4 - The text opens to Document View. Find a word that references a geographical location and double-click on it.

5 - In the small window that appears, click on the Places tab. It will auto-suggest a place location; if it is correct, click Confirm. These suggestions are often, however, hilariously wrong, and you will need to click Change.

6 - Type in the place name that is relevant for your annotated text, hit enter, and then select the linked database entry that best fits your location. Then click OK. \(If your text has other instances of that word, then it will ask you if you wish to apply the same annotation data to those other instances. You can do so if you know that they all in fact reference the exact same thing.\)

{% hint style="success" %}
**Example:** In an ancient Roman text, for a reference to Roman Italy I typed the Latin form ‘Italia’ to avoid getting only the modern country borders of ‘Italy’; for a reference to Emathia, a poetic term that in context means Thessaly rather than a specific place in Macedonia, I typed ‘Thessaly’.
{% endhint %}

7 - After doing the above step for as many place references in your text as you wish, go to the top and click on Map View to see the map generated from your annotations.

8 - To export your data, at the top click on Download Options.

## **How it works**

‌In order to place locations on a map, you need to assign it place coordinates \(in z/x/y format, e.g. elevation/latitude/longitude\). You could look up the real world coordinates for each location you want to map via Google Maps or other services, which can be a tedious process. This is the advantage of a tool like Recogito, since it can quickly collect that data for you.

Recogito works by adding already existing spatial data that resides in online databases with your selected word. There are several online gazetteers that Recogito relies on, a list of which can be found here \([https://recogito.pelagios.org/help/faq](https://recogito.pelagios.org/help/faq)\). For ancient world place data, it is best to rely on Pleiades \(‘P’\) or DARE \(the Digital Atlas of the Roman Empire = ‘D’\); for modern world place data, it is best to rely on GeoPlaces \(‘G’\).

It is thus worth keeping in mind that the spatial data that you link to your text is entirely reliant upon the nature of the information in these gazetteers. Some places you reference are mere points in space, others are polygon regions, all depending on how the database you use defines that location.

{% hint style="info" %}
INFO: ToposText \([https://topostext.org/](https://topostext.org/)\) is a another tool that links ancient texts \(with an emphasis on Greek literature\) with spatial maps, although it is more designed for identifying locations and seeing which texts mention a given place rather than creating your own exportable map data.
{% endhint %}

## **Further Resources**

\[suggestions?\]

