---
permalink: /introducing-gargoyle-poi-server/index.html
layout: post
title: Introducing Gargoyle POI Server
published: true
categories: []
---
Version 0.2 of the Gargoyle <acronym title="Point of Interest">POI</acronym> Server (GPS) is now ready.

The latest source code tarball is here: <a href="http://www.mockingeye.com/wp-content/uploads/2008/04/gargoyle_poi_server-02.tar.gz" title="Gargoyle POI Server v0.2">Gargoyle POI Server v0.2</a>. (Warning, almost no documentation and only basic comments)
Requirements: <a href="http://python.org/">python</a>, <a href="http://webpy.org/">web.py</a>, <a href="http://incubator.apache.org/couchdb/">CouchDB</a>, <a href="http://code.google.com/p/couchdb-python/">couchdb-python</a>

But, what is it?

A POI is a <a href="http://en.wikipedia.org/wiki/Point_of_interest">Point of Interest</a>. That is, it is an atomic element of geospatial information. The Gargoyle POI Server is the backend server to the Gargoyle Personal Agent (previously introduced under the name Gargoyle alone).

GPS is written in Python using <a href="http://webpy.org/">web.py</a> as the frontend, and <a href="http://incubator.apache.org/couchdb/">CouchDB</a> for data storage.  Web.py was chosen because it is small, fast, and output format agnostic. CouchDB provides schema-flexible storage and potential scalability. It will also support robust access from many Gargoyle Personal Agents (GPAs) as well multiple Gargoyle Extraction Agent Service (GEAS) instances.

At the moment, the system can output the POIs either in <a href="http://en.wikipedia.org/wiki/Keyhole_Markup_Language">KML</a> or in rudimentary HTML. The interface chosen is a simple <a href="http://en.wikipedia.org/wiki/REST">RESTful</a> interface. At the moment, only <code>GET</code> is supported. <code>POST</code> will be implemented soon.

Here is the syntax for using the server once running (to start a server at port 8080 just run <code>python locator.py</code>:

To view the POIs for <code>userid</code> in the square created by <code>45.000000,47.000000</code> and <code>45.000999,47.000999</code> (format is <code>latitude, longitude</code>)
<blockquote class="posterous_short_quote"><code>http://server:8080/l/userid/45.000/47.000</code></blockquote>
If you want it in KML use this:
<blockquote class="posterous_short_quote"><code>http://server:8080/l/userid/45.000/47.000?kml</code></blockquote>
To add a POI to <code>userid</code> with an expiration date on May 1st:
<blockquote class="posterous_short_quote"><code>http://server:8080/a/userid/45.000123/47.000456<em>/1.3</em>/POIname<em>/POI Description/2008-05-01</em></code></blockquote>
The third number is the Altitude. Optional elements are in italics, and include the altitude, the description, and the expiration date (default is 3 days). The <code>userid</code> can really be anything. Ideally, it's just a long-ish hash that can't be easily gussed. This simplifies access, and offers a measure of privacy. For now, if you want your POIs secret, you can encrypt their contents in whatever way you wish. Access control is planned, and will be implemented in a future version.

Coming <strong>really</strong> soon: GeoRSS output for easy Google Maps mashups.

For planned development, look at the upcoming Roadmap post.
