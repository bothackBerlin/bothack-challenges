# Lufthansa API
Miles and More – Loyalty Data Lufthansa Group data

## data
- **Member status:** `{GET}`<br>Loyalty status of the customer
- **Customer information:** `{POST}` **with PIN**<br>personal customer data, loyalty status and remaining loyalty points
- **Account statement:** `{GET}`<br>customer account statement with info for next loyalty level
- **Account balance:** `{GET}`<br>customer account balance

### memberAlias

| numbers | pin |
|---------|-----|
| 992002620696225<br>992004479235790<br>992005956306640<br>992002229864174<br>992000964979504<br>992000770952612<br>992001074776665<br>992005376147970<br>992000090543562<br>992001020426357 | 12345|

## data
### functionality
- **Earn Miles** `{POST}`<br>Credit miles onto a customer account
- **Spend Miles** `{POST}`<br>Post statement to debit miles onto a customer account

```
{
  "pid": 0, (leave it zero)
  "cardNo": "992002620696225", (member alias number)
  "action": "credit“, (fixed)
  "property": "MT002“, (fixed)
  "miles": 150000,
  "activityDate": "01.11.2016“, (DD.MM.YYYY)
  "transactionText": "Bothackathon“, ( String for account statement max 20char )
  "additionalPartnerData": „string“ (leave empty)
}
```

```
{
  "pid": 0, (immer null)
  "cardNo": "992001879787057“,
  "action": „debit“,  (Fix)  
  "awardCode": "ATES01“, (Fix)  
  "miles": 50,
  "statementText1": "Bothackathon“,( String for account statement max 20char ) "additionalPartnerData": „string“, (empty)
  "awardPackageId": „string“ (empty)
}
```
## Lufthansa group data
### Reference Data
- **City** by city code
- **Country** by country code
- **Airport** by airport code
- **Airlines** by airline
- **Nearest** Airport by geo
- **Aircraft** including Wifi

### Offers
- **Lounges** by airport
- **Seatmaps** per flight

### Operations
- **Live Flight Status**
- **Flight Schedule**

## How to reach the data
### Lufthansa Group Data
- **Token**<br>https://api.lufthansa.com/v1/oauth/token
- **plan**<br>open developer
- **data**<br>http://api.developer.com/(request)

- **Token**<br>https://api.lufthansa.com/v1/partners/oauth/token
- **plan**<br>Bothack Berlin
- **data**<br>https://api-test.developer.com/(request)

## Getting Started
1. Go to https://developer.lufthansa.com/
2. Register a user on the bottom of the page
3. Confirm the sign-up email

Register an service for **Bothack Berlin** and another app for **Open Developer plan!**<br>
Accept the ToS<br>
Ready to start on the API Playground with  **LH Partner TEST API**
