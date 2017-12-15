# Lab 03: Sequencing a Choropleth Map Through Temporal Data

## Part I. Building an interactive map (4 points)

Create an interactive web map of US unemployment rates by county. Use the map created within Lesson 03 as a guide.

Within the *lab-03/data/* directory, examine the *us-counties.json* file. Like the GeoJSON used in the lesson, it contains no quantitative attribute data, but merely a "GEOID" attribute which is each state and county FIPS code, concatenated together. You'll need to modify the script to bind the data to these geometries.

Also within the *lab-03/data/* directory is a data file, *us-unemployment-counties.csv*.

Begin by creating a new *index.html* file within the *lab-03/* directory.

Your map should fulfill the following requirements:

* Load two external files, a GeoJSON and a CSV, at runtime.
* Process these data, binding attribute data to geometries.
* Draw a classed choropleth map of unemployment rates for US counties using an appropriate classification method, e.g., ckmeans or quantile, or quartile and a sequential color scheme.
* Draw an accompanying legend with an appropriate legend title and class break labels.
* Display the map at 100% width and height of the browser window's viewport.
* Allow the user to zoom and pan.
* Provide a meaningful title for the map, placed upon the map.

In addition to these requirements, your map should also provide the following UI enhancements for the user:

* A visual affordance when the user hovers over specific counties (e.g., making the stroke of the county yellow).
* A tooltip triggered when the user clicks on a specific county, which provides the name of the county and the specific unemployment rate for the currently displayed year.

Finally:

* Thoroughly comment your code and commit your progress with meaningful commit messages as you work.

Your final map should look and behave like this:

![Final product for lab 03 assignment](graphics/lab-03-final.gif)

## Part II. Thinking deeply about data and map design (2 point critical reflection response)

Create a new file named *reflection.md* within your *lab-03/* directory and provide a short answer response (2 - 3 paragraphs) to the following question. This is a Markdown file, and you'll be writing plain text or Markdown.

Please understand that your choice of which "side" to pick is rhetorical for this assignment, may not reflect your own political viewpoint, and won't be reflected in the instructor's evaluation of your response. Sometimes it's a good exercise to consider a position you don't agree with!

**Question**: The meaning of this map can be interpreted in a number of ways, and the meaning of employment can be contextualized within greater socio-economic and political relations. How would you go about designing the map differently to support a general argument that the American economy is either "a complete disaster" or the "strongest, most durable in the world". Consider such aspects as:

* how "employment rates" are encoded by the raw data
* how the data are classified and represented thematically
* what information is included on the map (or left off)
* what marginalia or supplemental information you would include to help the user interpret the map
* how visual design elements could further promote the position of your client

Commit and save your changes to the *reflection.md* file and submit with your assignment by the due date.
