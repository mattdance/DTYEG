DTYEG
=====

<h1>Mapping Tutorial for Can You Dig It 2014</h1>
	<h2><a href="http://huco.ualberta.ca/">Digital Humanities Conference at the UofA</a></h2>

===================================
<p>This mapping tutorial has 4 components that cover three seperate platforms:
	<ol>
	<li>Open Street Map</li>
	<li>GitHub as a spatial data platform</li>
	<li>CartoDB - points and polygons</li>
	<li>CartoDB - temporal points</li>
	</ol>
</p>
<h2>Open Street Map</h2>
<p>OpenStreetMap (OSM) is a collaborative project to create a free editable map of the world. Two major driving forces behind the establishment and growth of OSM have been restrictions on use or availability of map information across much of the world and the advent of inexpensive portable satellite navigation devices.  OSM offers a couple of advantages:
<ol>
	<li>It is open sourced, so;</li>
	<li>The data is freely available;</li>
	<li>Regional Extracts can be found <a href="http://download.geofabrik.de/">here</a></li>
	<li>City Extracts can be found <a href="http://metro.teczno.com/">here</a></li>
</ol>	
We will be using OSM data for one of our mapping projects.
</p>

<h3>iD Editor</h3>
<p>
	The OSM iD Editor makes it easy to add spatial data.  I am not going to play this video here, but please reference back to this either later today when there is a break, or later later.
</p>
<p>
	MapBox has a great introduction to <a href="https://www.mapbox.com/blog/new-map-editor-launches-openstreetmap/">iD Editor</a>.
</p>

<h2>GitHub</h2>
<p>
	GitHub is a web-based hosting service for software development projects that use the Git revision control system.GitHub offers both paid plans for private repositories, and free accounts for open source projects. The site provides social networking functionality such as feeds, followers, wikis and the social network graph to display how developers work on their versions of a repository.
</p>

<p>
	The data that we will be working with are stored on GitHub as it offers an easy way to manage and visualise spatial data sets.
</p>

<p>
	Please have a look at and download the following data from Edmonton's downtown (Ward 6) onto your desktop.  You may choose to dump them into an unique folder:
	<ol>
		<li>Buildings. Data from OpenStreetMap.</li>
		<li>Surface Lots. Data from OpenStreetMap and Matt Dance.</li>
		<li>Boundary. Data from City of Edmonton.</li>
		<li>Trees. Data from City of Edmonton.</li>
	</ol>
</p>

C. Discuss the open data concept
D. Finding Spatial Data
	Often people want to make maps with data but just don't know where to start. While ideally you can upload some of your own data to CartoDB to play with, maybe you don't have data yet or are not sure where you would find the data you want. In those cases, it can be good to know some sites online to get good geospatial data.
	Here are a couple of our favorites:
	Natural Earth Data: data for borders, coastlines, cities, and many other useful collections!
	OpenStreetMap: here you can get many of the features that make up our cities, including polygons for neighborhoods and cities, roads, and even lampposts.
	Harvard Election Data Archive: we use this resource a lot. They keep a fantastic collection of elections data for races around the United States.
	The Global Biodiversity Information Facility: GBIF provides a portal to thousands of collections and millions of biodiversity records. If you want to map nature, there is no better place to start.

CartoDB - Points and Polygons

Credit - link to original

Summary
This tutorial will walk you through the basics of CartoDB. It is meant for beginners looking to get started using the platform but still uncertain where to begin. It is also a good tutorial to read through if you just want to know some basic functionality to get started.

Creating a new table
Uploading your own data is easy. We accept many common data formats such as CSV, Excel, ESRI Shapefiles, and GPX files. If you use SHP files, be sure to create a ZIP archive of all associated files (.shp, .prj, .dbx, etc) and upload the zip with all the files at once. To upload any supported file, either drag it directly onto the dashboard page of your CartoDB account, or click the Create your first table button, click 'select a file' and locate the file on your system, finally click 'Create table'.

Uploading data
Write intructions on how to upload these data above.


Creating a map
So now you have a dataset you are interested in mapping. Start by selecting the Map view, above your table. A map will appear, and your data will be rendered with the default styles. Okay! Points on a map, mission accomplished.

Our first map
Not so quick, let's look around. You can see above the map an option for changing the baselayer of your map. This won't change your data, but it sure can change how your data looks. Click on it and test some of the basemaps we provide as options.

Now let's explore some more options for map customization. To the right of the map you can see a toolbar with several buttons.

Almost at the top is the SQL option which allows you to perform SQL queries on your tables. This is not for us now, but CartoDB offers a tutorial on that <here>.

The next button is the Style option which gives you a menu for controlling the look of your visualizations. In this example, we can use options in the menu to change the fill color, width, stroke, labelling, etc. Play around with some of the settings to see what they do. By clicking the button again, you can close the interface and go back to seeing just your map.

Customization

Next is the Infowindow option, for customizing the contents of the infowindows that are shown when you click your data on the map. You can modify the style of the infowindow and the information that is shown. You can reorder the list of fields in your infowindows by simple drag & drop of the field names in the menu.
infowindows settings

Take your time playing with the options until you get familiar how map customization works in CartoDB.

Visualize your map
When you want to visualize different datasets or just share the map, you must create a visualization. Visualizations are where you will set and store all the filters and styles that you want to use in your published maps. Visualizations also let you add layers from multiple maps, mixing the data without having to write any complex code or queries. They also let you reuse data from the same tables in multiple visualizations without any difficulty. To get started with visualizations, click the orange Visualize button on the top right of the page. You will be prompted to add a name for your visualization, don't worry, you will be able to change it later.

visualize map
Visualizations are similar to tables, you can quickly tell them apart by looking at the icon beside the table name and the visualization name in the Table View. Now that you have created your visualization, it will be available on your dashboard.

Publish your map
Now that you have a Visualization just the way you want it, let's share it with some friends. Click the green Publish button in the top right of the page. From here you can customize how your published map is presented, including zoom and center, which interface elements to display, toggling layers, social media links, etc. At the bottom you will find a URL to share your Visualization via Twitter, email, or anywhere else. When you share that link, viewers will only be able to explore it on the map, they will not be able to edit any of your data. For more details, take a look at next tutorial.
publish map

Troque
Write this up myself.  What data do we want to viz?
