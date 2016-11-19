# <a name="challenge"></a>ING-DiBa data challenge
> Let’s admit it: Having to pay in cash is frustrating. But in our everyday life there are still many places and occasions where it is inevitable. Especially for Germans: They love their cash! Let’s take the pain out of „Damn, where do I get cash nearby?“.

## general dataset description
- ING-DiBa provides you with

## challenge description
- enable our customers to interact with their bank account – especially easing and managing their cash expenses. The chatbot should anticipating when our customers will need cash at hand and directing them to one of our preferred ATMs & partners - based on cash-forecast, geolocation and cash utilization


- address one or multiple of the following topics:
  - build a kind of financial management game for kids (adults) to learn how to spend, save and invest cash in the simple and smart way
  - simulate a fictitious incentive for using our own ATMs or spots to pick up cash from partners
  - help our customers managing their cash management and expenses due to their desires


- Failure resilience is one important evaluation criteria of your code base. The bot should fail gracefully if it’s not connected to the internet, if the API endpoints are not accessible, or if the API responses are not exactly as expected

### accessible datasources:
- some of the data below is available via a [REST API server](https://github.com/bothackBerlin/bothack-ing-diba-data-server).
- `atm.csv`
