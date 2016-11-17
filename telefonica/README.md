# Telefónica digital companion challenge
> We want to excel on our customer support by offering unique digital services along the entire customer journey – from when the need for a mobile contract first arises ’til it’s that time again.

## general dataset description
- Telefónica provides you with multiple platforms where you can request information from
- you find the detailed list and format description in tbd

## challenge description
- the goal of the challenge is that a chatbot enables our customers to experience any kind of informational request he would address to a customer service in a unique and compelling way by using the data sources provided and further 3rd party APIs


- address one or multiple of the following topics:
  - Finding the optimal Mobile Contract or Mobile Device for me or even my mom
  - Inspiring with content around mobile devices, offers, lifestyle, apps
  - Exploring the possibilities of a mobile device & the extending support
  - etc. just to become creative


- Failure resilience is one important evaluation criteria of your code base. The bot should fail gracefully if it’s not connected to the internet, if the API endpoints are not accessible, or if the API responses are not exactly as expected

### accessible datasources:
- `access.json` attached to access selfcare portal My O2
  - find nearby SIM cards for further usage
- `Targeting_Criterias.csv` attached to query from a simulated account
- information on:
  - social media:
    - https://twitter.com/o2de
    - https://www.facebook.com/o2Entdecken/
    - https://www.facebook.com/o2Hilfe/
    - https://www.instagram.com/o2deutschland
  - contracts and devices:
    - contracts `xml`
      - https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/tarife.xml
    - devices `xml`
      - https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/geraete.xml
    - combination `xml`
      - https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/bundles.xml
  - content `rss`:
    - o2 Forum: https://hilfe.o2online.de/community/feeds
      - Man kann auch spezielle RSS für Such-Abfragen erstellen auf https://hilfe.o2online.de/search
      Man kann die RSS auch für einzelne Subforen auslesen (IDs der Subforen anbei)
      § All Content Testgeräte & Testberichte: https://hilfe.o2online.de/community/feeds/allcontent?community=2127
      § Sub-Forum Testgeräte & Testberichte plus TagTestgeräte: https://hilfe.o2online.de/community/feeds/tags/testger%C3%A4t?community=2127
      § Neue Threads (ohne FAQs): https://hilfe.o2online.de/community/feeds/threads?community=2127
      § Neue Replies: https://hilfe.o2online.de/community/feeds/messages?community=2127
      § Unbeantwortete: https://hilfe.o2online.de/community/feeds/unansweredthreads?community=2127
      § Beliebte: https://hilfe.o2online.de/community/feeds/popularthreads?community=2127
    - https://www.o2online.de/blog/rss
    - news portal: https://curved.de/rss
  - crawler?
    - https://www.o2online.de
    - https://www.o2online.de/suche/consumer/
    - https://www.o2online.de/shops/ (alternative: 97% are indexed on GMaps)



  - net coverage
    - https://www.o2online.de/hilfe/o2-netz/
    - test case:
      - https://cdn2.spatialbuzz.com/api/coverage/2010-11-22/near/ctype/10/address/80992/customer/CSIEK3QbW2cyBiYOI3BcdhwxFF50UghXd10/auth/E1E1BD08:::79EC74A1?NoCache=60f85d49-93ae-823f-bdd4-716d72b33ccc&session_id=AjshADlSq2BO0xlln0VpwuSu9VPpBhdBRJmQa36EC-ox9DPbTgCSOyoDZnEocWW9



---

# Telefónica mobile lifestyle challenge
> Beyond offering an outstanding customer support we want to develop unique services that support our customer’s „mobile lifestyle“ – how can we create value beyond „the obvious“ and help our customers?

## general dataset description
- Telefónica provides you with

## challenge description
- The goal of the challenge is to rethink and redefine how our customers live their “mobile lifestyle” – as mobile connectivity becomes omnipresent – chatbots are the ideal companion to accompany our customers in their day-to-day life.


- Develop a Bot outside of our core business, that supports our users „mobile lifestyle“ using the data sources provided and 3rd party APIs available


- address one or multiple of the following use cases:
  - providing entertainment while on the go
  - offering location-based & personalized suggestions
  - support the customer while moving around in his own city or during travel

### accessible datasources:
- tbd
