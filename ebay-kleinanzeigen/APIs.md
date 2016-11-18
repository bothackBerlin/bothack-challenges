# Hack like a girl
You want to make it possible to get healthier while shopping? No Problem!

### The idea:
- An app where you can search for cool stuff close by.
- The app will show you where you find what you want and how much calories you will burn when you go there by foot, by bicycle or what you miss by going by car.
- Use eBay Kleinanzeigen to find ads which are close by the user and calculate the calories based on the distance


### [eBay Kleinanzeigen API](http://api.ebay-kleinanzeigen.de/docs/pages/home)
#### [Authentication](http://api.ebay-kleinanzeigen.de/docs/pages/security)
The API is secured by HTTPS and [HTTP basic auth](https://en.wikipedia.org/wiki/Basic_access_authentication). Use the following credentials to access it:
- take a look in the `secret.json`

#### [Response Format](http://api.ebay-kleinanzeigen.de/docs/pages/response-codes)
The eBay Kleinanzeigen API can return XML or Json formatted responses. The default is XML. To access the Json format append `.json` to the name of the endpoints below. Example: Instead of calling `/ads?q=iphone` call `/ads.json&q=iphone`. Please note that the Json has a quite irregular format.

#### [Perform a search](http://api.ebay-kleinanzeigen.de/docs/pages/ads)
Endpoint: **/ads**

#### Supported Parameters
| Parameter     | Description    |
| -------- | ----------------- |
| q | Search keyword (e.g. “iphone”) |
| categoryId | categoryId - See Retrieving Categories |
| latitude longitude distance | Parameters to perform a geo location based search. Latitude and Longitude define a point on the map and distance defines a circle around that point in km. All three parameters need to be supplied in order to make it work.
| minPrice | The minimum price you want to include in your search. |
| maxPrice | The maximum price you want to include in your search. |
| adType | Distinguish between people that offer items and those that are searching for items. |
| _in | A comma sperated list of fields that you want to be included in the response. This can be used to limit the response to fields that are relevant for your use case. Instead of showing all item details, you can limit the response to show for example only title and description. Options are for example description, title, pictures, search-distance |

#### Example: Search for an iPhone in whole Germany
[https://api.ebay-kleinanzeigen.de/api/ads?q=iphone](https://api.ebay-kleinanzeigen.de/api/ads?q=iphone)

#### Example: Search in the geo coordinates of Berlin with a radius of 4 km
[https://api.ebay-kleinanzeigen.de/api/ads?latitude=52.5200&longitude=13.4050&distance=4](https://api.ebay-kleinanzeigen.de/api/ads?latitude=52.5200&longitude=13.4050&distance=4)

When you perform a search that includes a geo position, the result will contain information about how far away each item is from the latitude and longitude that you provided.

```xml
<ad:ads>
  <ad:ad id="537527851">
    <ad:title>IKEA ALLAK * Bürostuhl * Drehstuhl * weiß * Kunstleder * günstig</ad:title>
    <ad:search-distance>
      <ad:distance>2.815145</ad:distance>
      <ad:distance-unit>
        <types:value>KM</types:value>
      </ad:distance-unit>
      <ad:display-distance>3 km</ad:display-distance>
    </ad:search-distance>
  </ad:ad>
  <ad:ad id="537527741">
    <ad:title>Winter Jacken</ad:title>
    <ad:search-distance>
      <ad:distance>2.753223</ad:distance>
      <ad:distance-unit>
        <types:value>KM</types:value>
      </ad:distance-unit>
      <ad:display-distance>3 km</ad:display-distance>
    </ad:search-distance>
  </ad:ad>
</ad:ads>
```

#### Retrieve all details of a single item
Endpoint: /ads

#### Retrieve Categories
Endpoint: /categories

You can retrieve the full category tree here
[categories docu](https://api.ebay-kleinanzeigen.de/api/categories)

Or retrieve details about only one category by providing a specific category id.
`https://api.ebay-kleinanzeigen.de/api/categories/{categoryId}``

### [eBay API](https://go.developer.ebay.com/)
The API: https://go.developer.ebay.com/

What you have to do:
-	Sign in for the developer program
-	Create a project
-	Create you keys: https://developer.ebay.com/my/keys
-	Start hacking

What can you do with it:
-	Finding API -> search for items & buy them
-	Shopping API -> search & buy & sell
Trading API -> buy & sell & transactions

![QR code](Picture1.png)
