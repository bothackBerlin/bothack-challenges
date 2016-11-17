# Hack like a girl
You want to make it possible to get healthier while shopping? No Problem!

### The idea:
- An app where you can search for cool stuff close by.
- The app will show you where you find what you want and how much calories you will burn when you go there by foot, by bicycle or what you miss by going by car.
- Use eBay Kleinanzeigen to find ads which are close by the user and calculate the calories based on the distance


### eBay Kleinanzeigen API
#### Authentication
The API is secured by HTTPS and [HTTP basic auth](https://en.wikipedia.org/wiki/Basic_access_authentication). Use the following credentials to access it:
- take a look in the access.js

#### Response Format
The eBay Kleinanzeigen API can return XML or Json formatted responses. The default is XML. To access the Json format append `.json` to the name of the endpoints below. Example: Instead of calling `/ads?q=iphone` call `/ads.json&q=iphone`. Please note that the Json has a quite irregular format.

#### Perform a search
Endpoint: **/ads**

#### Supported Parameters
[check out the docu](http://api.ebay-kleinanzeigen.de/docs/pages/home)


    + Example: Search for an iPhone in whole Germany
    + Example: Search in the geo coordinates of Berlin with a radius of 4 km
  + Retrieve all details of a single item
  + Retrieve Categories

### eBay API
