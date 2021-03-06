DTYEG
=====

<h1>Mapping Tutorial for Can You Dig It 2014</h1>


===================================
<p>Part of the <a href="http://huco.ualberta.ca/">Can You Dig It? 2014</a> Digital Humanities Conference at the UofA</p>

<p>We will be using <a href="http://cartodb.com/">CartoDB</a> as the mapping tool for this tutorial, so please, while we get going, head on over and sign up for a free account.</p>

<p>This mapping tutorial has 4 components that cover three seperate platforms:
	<ol>
	<li>Open Street Map</li>
	<li>GitHub as a spatial data platform</li>
	<li>CartoDB - points and polygons</li>
	<li>CartoDB - temporal points</li>
	</ol>
</p>
<p>
We will be using OSM data, in conjunction with <a href="https://data.edmonton.ca/">open data</a> from the City of Edmonton for this mapping project.
</p>
<p>
Also, you may want to reference my blog on <a href="http://www.matthewdance.ca/blog/neogeography/geoweb-tools/">How to make a web map.</a>
</p>


<h2>Open Street Map</h2>
<p>OpenStreetMap (OSM) is a collaborative project to create a free editable map of the world. Two major driving forces behind the establishment and growth of OSM have been restrictions on use or availability of map information across much of the world and the advent of inexpensive portable satellite navigation devices.  OSM offers a couple of advantages:
<ol>
	<li>It is open sourced, so;</li>
	<li>The data is freely available;</li>
	<li>OSM Regional Extracts can be found <a href="http://download.geofabrik.de/">here</a></li>
	<li>OSM City Extracts can be found <a href="http://metro.teczno.com/">here</a></li>
</ol>
</p>

<h3>OSM iD Editor</h3>
<p>
	The OSM iD Editor makes it easy to add spatial data.  I am not going to play this video here, but please reference back to this either later today, when there is a break, or later later.
</p>
<p>
	MapBox has a great introduction to <a href="https://www.mapbox.com/blog/new-map-editor-launches-openstreetmap/">iD Editor</a>.
</p>

<h2>GitHub</h2>
<p>
	GitHub is a web-based hosting service for software development projects that use the Git revision control system.GitHub offers both paid plans for private repositories, and free accounts for open source projects. The site provides social networking functionality such as feeds, followers, wikis and the social network graph to display how developers work on their versions of a repository. Git also offers an easy way to store and visualise spatial data.  We will explore more on this later.
</p>

<p>
	The data that we will be working with are stored on GitHub as it offers an easy way to manage and visualise spatial data sets.
</p>

<p>
	Please have a look at and download the following data from Edmonton's downtown (Ward 6) onto your desktop. The data are in the GitHub header, and we will do this together as I would like to show a couple of things.
	
	You may choose to dump them into an unique folder:
	<ol>
		<li>Buildings. Data from OpenStreetMap.</li>
		<li>Trees. Data from City of Edmonton.</li>
	</ol>
</p>

<h2>Open Data</h2>
<p>
"Open data is the idea that certain data should be freely available to everyone to use and republish as they wish, without restrictions from copyright, patents or other mechanisms of control." (from <a href"http://en.wikipedia.org/wiki/Open_data">Wikipedia</a>)
</p>
<p>
The City of Edmonton's <a href="https://data.edmonton.ca/">open data</a> portal is run a <a href="http://www.socrata.com/">Socrata</a>, also a mapping platform, and currently contains about 240 data sets.  While I think that the portal is great, it does not have any really high value data on it.  So, you should registr as a user, and request data sets.
</p>

<h2>CartoDB - Points and Polygons<h2>
<p>
With the goal of being 'open', I ripped most of this tutrial from CartoDB's <a href="http://developers.cartodb.com/tutorials.html">tutorial pages</a>. Also, look for CartoDB on Vimeo as they have some useful video tutorials.
</p>

<h3>Summary</h3>
<p>
This tutorial will walk you through the basics of CartoDB. It is meant for beginners looking to get started using the platform but still uncertain where to begin. It is also a good tutorial to read through if you just want to know some basic functionality to get started.
</p>

<h3>Creating a new table</h3>
<p>
Uploading your own data is easy. CartoDB accepts many common data formats such as CSV, Excel, ESRI Shapefiles, and GPX files. If you use SHP files, be sure to create a ZIP archive of all associated files (.shp, .prj, .dbx, etc) and upload the zip with all the files at once. To upload any supported file, either drag it directly onto the dashboard page of your CartoDB account, or click the Create your first table button, click 'select a file' and locate the file on your system, finally click 'Create table'.

Uplaod both the trees and buildings files.
</p>

<h3>Creating a map</h3>
<p>
So now you have datasets you are interested in mapping. Start by selecting the Map view, above your table. A map will appear, and your data will be rendered with the default styles. Okay! Points and polygons on a map, mission accomplished. Play with map views on both tables.
</p>

<h3>Our first map</h3>
<p>
Not so quick, let's look around. You can see above the map an option for changing the baselayer of your map. This won't change your data, but it sure can change how your data looks. Click on it and test some of the basemaps we provide as options.
</p>
<p>
Now let's explore some more options for map customization. To the right of the map you can see a toolbar with several buttons.
</p>
<p>
Almost at the top is the SQL option which allows you to perform SQL queries on your tables. This is not for us now, but CartoDB offers a tutorial on that.
</p>
<p>
The next button is the Style option which gives you a menu for controlling the look of your visualizations. In this example, we can use options in the menu to change the fill color, width, stroke, labelling, etc. Play around with some of the settings to see what they do. By clicking the button again, you can close the interface and go back to seeing just your map.
</p>

<h3>Customization</h3>
<p>
Next is the Infowindow option, for customizing the contents of the infowindows that are shown when you click your data on the map. You can modify the style of the infowindow and the information that is shown. You can reorder the list of fields in your infowindows by simple drag & drop of the field names in the menu.
</p>
<p>
Take your time playing with the options until you get familiar how map customization works in CartoDB.
</p>

<h3>Visualize your map</h3>
<p>
When you want to visualize different datasets or just share the map, you must create a visualization. Visualizations are where you will set and store all the filters and styles that you want to use in your published maps. Visualizations also let you add layers from multiple maps, mixing the data without having to write any complex code or queries. They also let you reuse data from the same tables in multiple visualizations without any difficulty. 
</p>
<p>
To combine and visualise your two tables, select one map to work from, and simply click the "+" button at the top of the sliding menu drawer and select your other table.
</p>

<p>
Visualizations are similar to tables, you can quickly tell them apart by looking at the icon beside the table name and the visualization name in the Table View. Now that you have created your visualization, it will be available on your dashboard.
</p>

<h3>Publish your map</h3>
<p>
Now that you have a Visualization just the way you want it, let's share it with some friends. Click the green Publish button in the top right of the page. From here you can customize how your published map is presented, including zoom and center, which interface elements to display, toggling layers, social media links, etc. At the bottom you will find a URL to share your Visualization via Twitter, email, or anywhere else. When you share that link, viewers will only be able to explore it on the map, they will not be able to edit any of your data. For more details, take a look at next tutorial.
publish map
</p>

<h1>Torque</h1>
<p>
If we have some time, we can play with Torque, an easy way to visualise time series data.
</p>

