# GWU Project #2 
*Project by: Sania Ahmad, Haris Nawzadi, Sobaid Zewari*

**Project Outline:**
For our project we created a website that sighting opportunities of the International Space Station (ISS) in cities near where we live. The data includes date, time, location, and amount of time the station is visible.  Additionally, created a live tracker that shows where the ISS is at any given moment around the world, and allows for the users interactively explore the map.
 
**Importing the data into a Database:**
We began by creating a SQL database, called ISS_Locations where we imported our CSV file. Our CSV file contains the general location in the sky when the ISS can be visible on a given date in a given city. The cities include Northern Virginia. Maryland, and DC. 

See Python Code [HERE](https://github.com/saniaahmad9/ProjectTwo/blob/master/Project-2.v2/JavaScript-master/Untitled.ipynb)

**SQL Alchemy and Flask:**
We used SQL Alchemy to create the connection string to the database, created the application object, and specified our routes. We had four routes, one for our homepage, one for our data page, one for our live tracker page, and one that returns our data as a JSON. This last route required us to query the database, create a dataframe from the data, and JSONify the data to be used in the app.js file. 

**Javascript and d3:**
We used d3.json to capture the JSONified version of our data from the last route created. We then built the table. This involved looping through each object in the data and appending a row and cells for each value in the row. 

View our 

![Space Station](https://www.nasa.gov/sites/default/files/styles/full_width_feature/public/thumbnails/image/iss044e045215_lrg.jpg)
