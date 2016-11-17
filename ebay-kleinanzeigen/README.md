# eBay data challenge
> We want to help our customers – buyers & sellers – to make better pricing decisions when purchasing or selling an item on our platform: eBay Kleinanzeigen. Is it the right time to sell the product now or would I get a better price next week? Is this price ok or am I paying too much? Should I add something to my ad to get a better price?

## general dataset description
- eBay Kleinanzeigen provides you their full API. You can find their price finder [here](http://preisfinder.ebay-kleinanzeigen.de/) and their favourite search [here](https://www.ebay-kleinanzeigen.de/s-beliebte-suchen.html)

## challenge description
- the goal of the challenge is to enable our customers to come to the best decision for purchasing items by using the provided data sources and 3rd party APIs


- address one or multiple of the following topics:
  - Finding the optimal moment to purchase or sell an item  
  - Finding the optimal price to purchase or sell an item for
  - Receiving hints to optimize your ad to increase performance
  - Receiving valuable information on purchased products
  - Accessing 1st Level Support through messaging


- Failure resilience is one important evaluation criteria of your code base. The bot should fail gracefully if it’s not connected to the internet, if the API endpoints are not accessible, or if the API responses are not exactly as expected

### accessible datasources:
- check [API.md](API.md)
