---
title: Census 2011 by the county and Fusion Tables, mapping the data.
author: Colin Broderick
layout: post
permalink: /2011/07/census-2011-by-the-county-and-fusion-tables-mapping-the-data/
dsq_thread_id:
  - 371206737
categories:
  - Of Interest
  - Regional Development
tags:
  - Census 2011
  - Fusion Tables
  - GIS
  - Ireland
  - Population
  - Quantum GIS
---
Well the preliminary Census 2011 data has been out over a week not and thankfully i have finally figured out how to make a map using [googles new fusion tables service][1]. My inspiration came from the [Guardians Data Blog][2].

All the materials required a freely available. The CSO provide some shapefiles of the areas which they use to reference the data, I was after the file that had the county council area data in it, which you can find in the [electoral division file][3]. It&#8217;s an [ESRI Shapefile][4] and they don&#8217;t work in Fusion Tables out of the box.

So next step is to convert the file to a KML (keyhole markup language) you may recognize the file type from the files you load in to google earth. In order to this if you have loads of money you can use [ArcMap][5] or my case I don&#8217;t get over to the [QuantumGIS site][6] and download it! Its the &#8220;user friendly Open Source Geographic Information System&#8221;.

The electoral division file uses the Irish Grid projection so you need to set this correctly in QGIS and then right click the layer and save as a kml file with the WGS84 crs in order for it to show in the right location on Google Maps. One other note is you will have to strip out the electoral divisions and just leave the county boundaries too. What you&#8217;re left with looks like this:

<div id="attachment_1518" class="wp-caption aligncenter" style="width: 522px">
  <a href="{{site.baseurl}}/wp-content/uploads/2011/07/Screen-shot-2011-07-07-at-21.29.46.png"><img class="size-full wp-image-1518 " title="Ireland ED shapefile" src="{{site.baseurl}}/wp-content/uploads/2011/07/Screen-shot-2011-07-07-at-21.29.46.png" alt="" width="512" height="602" /></a><p class="wp-caption-text">
    Ireland ED shapefile
  </p>
</div>

I downloaded the county data from the Census tables on the [CSO website][7], get them form **Table 1**. Put them in a google spreadsheet and load them into fusion tables while also uploading your exported kml file as well. Once you merge them you end up with a table like this:

[<img class="alignleft size-large wp-image-1507" title="Census 2011 Fusion Table" src="{{site.baseurl}}/wp-content/uploads/2011/07/Screen-shot-2011-07-07-at-21.10.31-1024x350.png" alt="" width="1024" height="350" />][8]

&nbsp;

The nifty part of fusion tables is that you can just click a button and it will plot all this data onto a Google Map. The result of which is below, if you would like to have a look at the table, either click on the image above which links to it or [Census 2011 Mapped by County][8]. Can some one please let me know if this is breaking some license as regards the use of the data, because i&#8217;m not too sure what the license is.

&nbsp;



Let me know what you think in the comments below.

# Don&#8217;t forget!

As always folks comments are welcome, you can follow me on the tweet machine **<a title="Follow me on Twitter" href="http://twitter.com/#!/rusty1052" target="_blank">@Rusty1052</a>**. Only want the blog? Subscribe to the **<a title="RSS Feed" href="http://feeds.feedburner.com/AnIrishPlanningStudentsBlog" target="_blank">RSS Feed</a>** with your favorite reader!

Toodles!

<span class='st\_twitter\_vcount' st\_title='Census 2011 by the county and Fusion Tables, mapping the data.' st\_url='{{site.baseurl}}/2011/07/census-2011-by-the-county-and-fusion-tables-mapping-the-data/' displayText='share'></span><span class='st\_fblike\_vcount' st\_title='Census 2011 by the county and Fusion Tables, mapping the data.' st\_url='{{site.baseurl}}/2011/07/census-2011-by-the-county-and-fusion-tables-mapping-the-data/' displayText='share'></span><span class='st\_plusone\_vcount' st\_title='Census 2011 by the county and Fusion Tables, mapping the data.' st\_url='{{site.baseurl}}/2011/07/census-2011-by-the-county-and-fusion-tables-mapping-the-data/' displayText='share'></span><span class='st\_sharethis\_vcount' st\_title='Census 2011 by the county and Fusion Tables, mapping the data.' st\_url='{{site.baseurl}}/2011/07/census-2011-by-the-county-and-fusion-tables-mapping-the-data/' displayText='share'></span>

 [1]: http://www.google.ie/url?sa=t&source=web&cd=1&sqi=2&ved=0CCgQqwMoADAA&url=http%3A%2F%2Fwww.google.com%2Ffusiontables%2Fpublic%2Ftour%2Findex.html&ei=vRMWTo_zL8SKhQfJ5Oxj&usg=AFQjCNG1nPT3B1RSytOBX8ZhlrQYlqupJw
 [2]: http://www.guardian.co.uk/data
 [3]: http://census.cso.ie/censusasp/saps/boundaries/eds_bound.htm
 [4]: http://en.wikipedia.org/wiki/Shapefile "Explains what it is!"
 [5]: http://www.esri.com/products/index.html#desktop_gis_panel
 [6]: http://www.qgis.org/
 [7]: http://www.cso.ie/census/2011_preliminaryreport.htm
 [8]: http://www.google.com/fusiontables/DataSource?snapid=S218835h8Us