---
permalink: /progress-on-gargoyle/index.html
layout: post
title: Progress on Gargoyle
published: true
categories: []
---
Remember <a href="http://www.mockingeye.com/index.php/2007/12/12/introducing-gargoyle-the-geospatial-web-in-your-pocket/">Gargoyle</a>?

Well, it hasn't been abandoned yet. I've been rewriting the design and scrapping it over and over. I think I've finally reached a design that's stable, and that will plug nicely into all kinds of stuff.

Today I wrote a lightweight <a href="http://new.webpy.org/">web.py</a>-based <a href="http://en.wikipedia.org/wiki/Point_of_Interest">POI</a> system. It gives a user a random hash which is used to identify a unique POI list. Access is done <a href="http://en.wikipedia.org/wiki/Representational_State_Transfer">RESTfully</a>. That is:

<blockquote class="posterous_short_quote">
<code>http://www.example.com/locate/te6hemi8t3cu/38.89768/-77.036455/</code>
</blockquote>

Which would display all POIs in the list <code>te6hemi8t3cu</code> that are in the box bounded by <code>(38.897000, -77.036000)</code> and <code>(38.897999, -77.036999)</code>. That is, three spaces after the decimal is my chosen granularity (it's roughly walking distance). The POI list is produced either in a human readable bullet-point list (for easy display on mobile devices), or as a <a href="http://en.wikipedia.org/wiki/Keyhole_Markup_Language">KML</a> file (with some added metadata of course. Such as an expiration date for the entry).

Adding a POI is just as easy, just using <code>add</code> instead of <code>locate</code>, and appending <code>/poi_info</code> to the URL.

This means that you can easily write apps to use this simple API, as well as display it using Google Earth.

What's the next step? I need to convert my already existing client for the Nokia N800 to be able to use this POI list, as well as maintain its own POI cache. It should only read to the user things within a 4 or 5 decimal space distance, and not bother querying unless the user is approaching the edges of the grid box she's in.

Finally, once these infrastructure issues are taken care of, the real purpose of Gargoyle will be implemented. This takes the form of a the app that goes through your "reading list" and adds relevant items to the POI list. 

I will post the code for the N800 code and the POI server some time within the week. It still needs some cleanup. Gargoyle v0.2 here we come!

<strong>Addendum:</strong> POIs can also be meta-POIs. That is, rather than being a placename, an entry into the db can be a uri to an external kml source (can be dynamic). An example would be a URL that points to a script that forwards the coords to the <a href="http://www.geonames.org/export/wikipedia-webservice.html">Geonames Wikipedia web service service</a> (shows nearest wikipedia entries) and converts the resulting XMl or JSON into KML.
