# Restaurant-location-Analysis
## Introduction/Business Problem

  One of the most common and profitable businesses are Restaurants. In order to have a successful restaurant, one must choose the best location possible. Having a good menu and professional staff is important, but having a good location can give your business another push toward success.
  
![alt text](https://cdnimg.webstaurantstore.com/uploads/buying_guide/2014/10/rla-waiter.jpg)

 The aim of this project is to perform a location analysis for a new restaurant; For a given city, what is the best location possible to open a restaurant? We will use the city of Toronto, Canada as an example.
 There are many details that we should look into when it comes to making the choice of the best location:
 
 * Access
 * Proximity to Suppliers
 * Competition
 * Visibility
 
 In this project, we will focus only on the competition aspect. 
 
 ## Data 
 
 In order to solve this problem, we will use Foursquare API for location data. For the Toronto neighborhood data, a Wikipedia page exists that has all the information we need. We will scrape this page and wrangle the data, clean it, and then read it into a pandas dataframe so that it is in a structured format before putting it to use.
 
 ## Methodology
 The steps are as following:
 
 1. Data extraction and cleaning
 2. Preprocessing neighborhood data
 3. Analyzing neighborhoods and finding the neighorhoods with the biggest number of restaurants
 4. Predicting the best restaurant locations
 
We used this website (https://cocl.us/Geospatial_data) in order to extract geospatial data in order to explore the neighborhoods using Foursquare. This is an example of what could be exctracted from the Wikipedia page and this website:

![alt text](https://github.com/Marwanegoudani/Restaurant-location-Analysis/blob/master/example_data.png)

We used KMeans in order to cluster the neighborhoods and determine the best neighborhoods for a new restaurant. Those are the neighborhoods that offer the best competition, meaning those who have the biggest number of restaurants.

## Results 
The results were as follows.
![alt text](https://github.com/Marwanegoudani/Restaurant-location-Analysis/blob/master/example_data.png)
The red marks correspond to the best locations to open a restaurant.
They are the neighborhoods that offer the best competition and thus a free marketing and an easy access.
We notice that these locations are closer to the sea than the other, which is explained by the fact that the sea attracts more people and the neighborhoods that are close to it are the most crowded.
