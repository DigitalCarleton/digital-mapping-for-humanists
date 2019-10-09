# Building a spreadsheet for location data

## **Introduction**

This recipe will provide some basic principles and best practices for creating a spreadsheet which will easily translate into a .csv file for import into the mapping application of your choice.

## **Ingredients**

A spreadsheet application \(e.g. Microsoft Excel, Google Sheets, Airtable.com, etc.\)

## **How to do it**

1. Decide what information you want your map to communicate. This determination will be invaluable as you gather your data, and will also eventually translate into the columns/fields on your spreadsheet which will be used to classify your data. To help you with this task, it would be beneficial to consider the pre-mapping questions available in the “[Digital Mapping Questionnaire](https://docs.google.com/document/d/1TvKZvA00E-OvGpRqsBwCuAeUmPl2p62hkLPCezE90o0)” recipe.
2. Open your spreadsheet application and create a new project.
3. Name your columns/fields \(located along the top of your spreadsheet\) according to the specific attributes of your data which you are tracking and wish to communicate. In Microsoft Excel and Google Sheets, these labels should go in row 1. In other applications such as Airtable, columns/fields are named directly, leaving row 1 open for your data.

{% hint style="info" %}
**Best practice tips:**

* When naming your columns and fields, avoid spaces by using naming conventions such as camelCase or snake\_case.
* Try to limit your labels to 9 characters or fewer. Some mapping applications into which you may end up importing your data have a tendency to truncate values beyond 9 characters, which can result in the appearance of duplicate values.
* Avoid the use of special characters \(e.g. \*, ?, /, $\) and accent marks.
{% endhint %}

4. Two of your columns/fields should be named “Latitude” and “Longitude,” assuming you will be using such coordinates for placing points on your map. Some mapping applications will automatically be able to detect these fields for what they are if the names are typed out and not abbreviated \(e.g. “lat” and “long”\).

{% hint style="info" %}
**Best practice tips:**

* When entering latitude and longitude coordinates, it is usually best to use a decimal value \(e.g. 41.887060, -87.634160\) rather than the degrees/minutes/seconds \(DMS\) format. There are a number of online tools which will convert DMS to decimal for you if needed, such as the one at [https://www.fcc.gov/media/radio/](https://www.fcc.gov/media/radio/dms-decimal)[dms-decimal](https://www.fcc.gov/media/radio/dms-decimal).
* For more information on how to get latitude and longitude coordinates, see the [CSV File Subrecipe: Finding Latitude and Longitude for a Location; Working with locational data](https://docs.google.com/document/d/1a0_jbx-2t1hBjgC-4SJCMC5Z5a0DlxUWkP-Rom8AbRA).
{% endhint %}

5. Other columns/fields should simply help you classify your data.

{% hint style="info" %}
**Best practice tip:**

* In general, try to keep each individual column/field as singular as possible; that is, try not to have one column/field tell you multiple things about your data.
{% endhint %}

6. When your data is ready, save or export it into the .csv \(comma separated values\) format. This is a basic, versatile file format which most other spreadsheet and mapping applications should be able to read.

{% hint style="info" %}
**Best practice tip:**

* If you are using Microsoft Excel, there are a number of different .csv options you can use when saving your document, but some of them can result in formatting which is not as friendly to import into other applications. In general, the “CSV \(Comma delimited\) \(\*.csv\)” option should work well. If you find that you have problems with that one, you could try “CSV UTF-8 \(Comma delimited\) \(\*.csv\)” option instead.
{% endhint %}

## **Further Resources**

**Spreadsheet applications**

* \*\*\*\*[Microsoft Excel](https://products.office.com/en-us/excel) \($\)
* [Google Sheets](https://www.google.com/sheets/about/) \(free\)
* [Airtable.com](https://airtable.com/) \(free w/ subscription options\)

**Add-ons and plugins**

* \*\*\*\*[Geocode by Awesome Table](https://sites.google.com/site/scriptsexamples/available-web-apps/awesome-tables/add-ons/geocode) -- A free add-on for Google Sheets which will get longitude and latitude data from a list of physical addresses.

