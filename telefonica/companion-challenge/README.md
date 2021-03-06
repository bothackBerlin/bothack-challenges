# <a name="challenge-1"></a>Telefónica digital companion challenge <img align="right" alt="bothack.berlin Logo" src="../Logos-Telefonica-o2-300dpi.jpg" width="200" />
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
- some of the data below is available via a [REST API server](https://github.com/bothackBerlin/bothack-telefonica-data-server).
- information on:
  - social media:
    - https://twitter.com/o2de
    - https://www.facebook.com/o2Entdecken/
    - https://www.facebook.com/o2Hilfe/
    - https://www.instagram.com/o2deutschland
  - simulate your own account data based on the format provided in [targeting_criterias.csv](./targeting_criterias.csv).
  - contracts and devices:
    - contracts: [tarife.xml][tarife_xml-local] ([source][tarife_xml-remote])
    - devices: [geraete.xml][geraete_xml-local] ([source][geraete_xml-remote])
    - combination: [bundles.xml][bundles_xml-local] ([source][bundles_xml-remote])
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
  - crawler
    - https://www.o2online.de
    - https://www.o2online.de/suche/consumer/
    - https://www.o2online.de/shops/ (alternative: 97% are indexed on GMaps)



  - net coverage
    - https://www.o2online.de/hilfe/o2-netz/
    - test case:
      - https://cdn2.spatialbuzz.com/api/coverage/2010-11-22/near/ctype/10/address/80992/customer/CSIEK3QbW2cyBiYOI3BcdhwxFF50UghXd10/auth/E1E1BD08:::79EC74A1?NoCache=60f85d49-93ae-823f-bdd4-716d72b33ccc&session_id=AjshADlSq2BO0xlln0VpwuSu9VPpBhdBRJmQa36EC-ox9DPbTgCSOyoDZnEocWW9

[tarife_xml-local]: ./tarife.xml
[tarife_xml-remote]: https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/tarife.xml
[geraete_xml-local]: ./geraete.xml
[geraete_xml-remote]: https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/geraete.xml
[bundles_xml-local]: ./bundles.xml
[bundles_xml-remote]: https://www.o2online.de/eshop/static/rest/xmlfeeds/v4/o2shop/bundles.xml
