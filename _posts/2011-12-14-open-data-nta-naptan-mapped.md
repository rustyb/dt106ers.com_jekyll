---
title: '[OPEN DATA] NTA NaPTAN Mapped'
author: Colin Broderick
layout: post
permalink: /2011/12/open-data-nta-naptan-mapped/
dsq_thread_id:
  - 504397511
categories:
  - Of Interest
  - Transport
tags:
  - Dublin
  - Dublin Bus
  - DubLinked
  - Fusion Tables
  - google
  - Ireland
  - National Transport Authority
  - Open Data
  - Transport
---
A quick post today showing just the sort of data that has been made available through the [DubLinked][1] project. I attended the recent DubLinked workshop in IBM themed around planning data. It was great fun had some serious chats with [@josephcorr][2] and [@Fingal\_Data\_Hub][3] on the upcoming <a href="http://data.fingal.ie/apps4fingal/" target="_blank">#Apps4Fingal</a> competition, and no I have not come up with a proper proposal yet.

Any who that aside it was announced that the <a href="http://nationaltransport.ie" target="_blank">National Transport Authority</a> had made one of their datasets available fo public consumption. This particular dataset is that of all the transport stops in the country, and for those transport planners/traffic engineers among us will know theses are the <del>same nodes used in the Greater Dublin Area Saturn Model for travel and transport</del>. **[Update] [As per Peter&#8217;s comment below][4]: &#8220;The transit access nodes used in the NTA Saturn Model are not the bus stops in NaPTAN, but rather access to public transport is generalised to road junction nodes.&#8221;**

So basically to break it down the data is a rather large xml file which contains all the points (the individual stops and stop areas) and a .mbd file containing what i presume is service information. Unfortunately I can&#8217;t open that one as I don&#8217;t have microsoft access on the mac. So if someone can open it I would love to hear what is in the file.

Right long long story short I parsed the xml file into a csv file and uploaded it to the great <a href="http://google.com/fusiontables" target="_blank">fusion tables</a> and below is the result. There are a few problems with the data in that if you zoom out you will see stops are mapped all over the world! This I reckon is a result of a portion of the co-ordinates not being projected in WSG84 as they are probably in Irish Grid form.

## NTA NaPTAN Data Mapped



Just for a small bit of brevity if you&#8217;re wondering what the hell a Stop Type of BCT means check out this handy reference from the <a href="http://www.dft.gov.uk/naptan/stopTypes.htm" target="_blank">Department for Transport, UK</a>.

## NaPTAN Stop Types

<table>
  <tr>
    <th>
      Value
    </th>
    
    <th>
      Description
    </th>
    
    <th>
      Nat
    </th>
    
    <th>
    </th>
    
    <th>
      Mode
    </th>
    
    <th>
      Type
    </th>
    
    <th>
      Version
    </th>
  </tr>
  
  <tr>
    <td rowspan="4">
      BCT
    </td>
    
    <td rowspan="4">
      On-street Bus / Coach / Tram Stop
    </td>
    
    <td rowspan="4">
    </td>
    
    <td rowspan="6">
      On street
    </td>
    
    <td rowspan="4">
      BusCoach
    </td>
    
    <td>
      MarkedPoint
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      UnmarkedPoint
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      HailAndRide
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      FlexibleZone
    </td>
    
    <td>
      2.0
    </td>
  </tr>
  
  <tr>
    <td>
      TXR
    </td>
    
    <td>
      Taxi Rank (head of)
    </td>
    
    <td>
    </td>
    
    <td rowspan="2">
      Taxi
    </td>
    
    <td>
      TaxiRank
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      STR
    </td>
    
    <td>
      Shared Taxi Rank (head of)
    </td>
    
    <td>
    </td>
    
    <td>
      SharedTaxiRank
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      AIR
    </td>
    
    <td>
      Airport Entrance
    </td>
    
    <td>
    </td>
    
    <td rowspan="15">
      Off street
    </td>
    
    <td rowspan="2">
      Air
    </td>
    
    <td>
      Entrance
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      GAT
    </td>
    
    <td>
      Airport Interchange Area
    </td>
    
    <td>
      920
    </td>
    
    <td>
      AccessArea
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      FTD
    </td>
    
    <td>
      Ferry Terminal / Dock Entrance
    </td>
    
    <td>
      930
    </td>
    
    <td rowspan="3">
      Ferry / Ship
    </td>
    
    <td>
      Entrance
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      FBT
    </td>
    
    <td>
      Ferry or Port Berth
    </td>
    
    <td>
      930
    </td>
    
    <td>
      Berth
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      FER
    </td>
    
    <td>
      Ferry or Port Interchange Area
    </td>
    
    <td>
      930
    </td>
    
    <td>
      AccessArea
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      RSE
    </td>
    
    <td>
      Rail Station Entrance
    </td>
    
    <td>
    </td>
    
    <td rowspan="3">
      Rail
    </td>
    
    <td>
      Entrance
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      RLY
    </td>
    
    <td>
      Railway Interchange Area
    </td>
    
    <td>
      910
    </td>
    
    <td>
      AccessArea
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      RPL
    </td>
    
    <td>
      Railway Platform
    </td>
    
    <td>
      910
    </td>
    
    <td>
      Platform
    </td>
    
    <td>
      1.2
    </td>
  </tr>
  
  <tr>
    <td>
      TMU
    </td>
    
    <td>
      Tram / Metro / Underground Entrance
    </td>
    
    <td>
    </td>
    
    <td rowspan="3">
      Tram / Metro
    </td>
    
    <td>
      Entrance
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      MET
    </td>
    
    <td>
      Underground or Metro Interchange Area
    </td>
    
    <td>
      940
    </td>
    
    <td>
      AccessArea
    </td>
    
    <td>
      1.2
    </td>
  </tr>
  
  <tr>
    <td>
      PLT
    </td>
    
    <td>
      Underground or Metro platform
    </td>
    
    <td>
      940
    </td>
    
    <td>
      Platform
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      BCE
    </td>
    
    <td>
      Bus / Coach Station Entrance
    </td>
    
    <td>
    </td>
    
    <td rowspan="4">
      BusCoach
    </td>
    
    <td>
      Entrance
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      BST
    </td>
    
    <td>
      Bus Coach Station Access Area
    </td>
    
    <td>
      900
    </td>
    
    <td>
      AccessArea
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      BCS
    </td>
    
    <td>
      Bus / Coach bay / stand /<br /> stance within Bus / Coach Stations
    </td>
    
    <td>
      900
    </td>
    
    <td>
      Bay
    </td>
    
    <td>
      1.0
    </td>
  </tr>
  
  <tr>
    <td>
      BCQ
    </td>
    
    <td>
      Bus Coach Station Variable Bay
    </td>
    
    <td>
      900
    </td>
    
    <td>
      VariableBay
    </td>
    
    <td>
      2.0
    </td>
  </tr>
</table>

**Source:** <a href="http://www.dft.gov.uk/naptan/stopTypes.htm" target="_blank">http://www.dft.gov.uk/naptan/stopTypes.htm</a>

&nbsp;

## As always!

Comments are welcome, you can follow me on the tweet machine **<a title="Follow me on Twitter" href="http://twitter.com/#!/rusty1052" target="_blank">@Rusty1052</a>**. Only want the blog? Subscribe to the **<a title="RSS Feed" href="http://feeds.feedburner.com/AnIrishPlanningStudentsBlog" target="_blank">RSS Feed</a>** with your favorite reader!

Do you like what you have just read? Maybe you are interested in being a guest writer too. Email me at colinb@dt106ers.com

<span class='st\_twitter\_vcount' st\_title='[OPEN DATA] NTA NaPTAN Mapped' st\_url='{{site.baseurl}}/2011/12/open-data-nta-naptan-mapped/' displayText='share'></span><span class='st\_fblike\_vcount' st\_title='[OPEN DATA] NTA NaPTAN Mapped' st\_url='{{site.baseurl}}/2011/12/open-data-nta-naptan-mapped/' displayText='share'></span><span class='st\_plusone\_vcount' st\_title='[OPEN DATA] NTA NaPTAN Mapped' st\_url='{{site.baseurl}}/2011/12/open-data-nta-naptan-mapped/' displayText='share'></span><span class='st\_sharethis\_vcount' st\_title='[OPEN DATA] NTA NaPTAN Mapped' st\_url='{{site.baseurl}}/2011/12/open-data-nta-naptan-mapped/' displayText='share'></span>

 [1]: http://www.dublinked.ie/ "DubLinked Website"
 [2]: http://twitter.com/#!/josephcorr
 [3]: http://twitter.com/#!/Fingal_Data_Hub
 [4]: {{site.baseurl}}/2011/12/open-data-nta-naptan-mapped/#comment-386787002