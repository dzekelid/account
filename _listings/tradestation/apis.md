---
name: TradeStation
x-slug: tradestation
description: Whether you trade stocks, ETFs, options or futures, TradeStation???s
  award-winning tools and brokerage services can give you the confidence to achieve
  your goals.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
x-kinRank: "7"
x-alexaRank: "37688"
tags: Account
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/apis.md
specificationVersion: "0.14"
apis:
- name: Tradestation API - Get Account Orders
  x-api-slug: accountsaccount-keysorders-get
  description: |-
    Returns the Orders for the given accounts sorted descending, most recent order first.

    #### Stateless Connection
    Since the web-API provides a stateless connection, it only supports fetching the current state of Orders. If it is needed to display the intermediate state changes, it should be executed at client level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keysorders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keysorders-get-openapi.md
- name: Tradestation API - Get Account Positions
  x-api-slug: accountsaccount-keyspositions-get
  description: Returns the Positions for the given accounts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keyspositions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keyspositions-get-openapi.md
- name: Tradestation API - Get Account Balances
  x-api-slug: accountsaccount-keysbalances-get
  description: Returns the Balance for the given accounts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keysbalances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/tradestation/accountsaccount-keysbalances-get-openapi.md
x-common:
- type: x-website
  url: http://www.tradestation.com
- type: x-api-gallery
  url: http://tigertext.api.gallery.streamdata.io
- type: x-api-stack
  url: http://tradestation.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/tradestation-technologies
- type: x-developer
  url: https://developer.tradestation.com/
- type: x-documentation
  url: https://tradestation.github.io/api-docs/
- type: x-faq
  url: https://www.tradestation.com/faq/
- type: x-github
  url: https://github.com/tradestation
- type: x-openapi
  url: https://tradestation.github.io/api-docs/swagger.json
- type: x-pricing
  url: https://www.tradestation.com/pricing/
- type: x-twitter
  url: https://twitter.com/TradeStation
- type: x-website
  url: https://www.tradestation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---