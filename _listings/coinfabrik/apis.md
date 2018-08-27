---
name: CoinFabrik
x-slug: coinfabrik
description: Our smart contract development and full stack blockchain development
  services are supported by more than 20 years of experience building and reviewing
  secure applications. CoinFabrik is a full stack blockchain development company.
  Our expertise range from extending cryptocurrency nodes like Bitcoin and Ethereum
  to providing high level APIs and UIs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
x-kinRank: "7"
x-alexaRank: "970321"
tags: Account
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/apis.md
specificationVersion: "0.14"
apis:
- name: Coinbase API - Set account as primary
  x-api-slug: accountsaccount-idprimary-get
  description: Promote an account as primary account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/accountsaccount-idprimary-get-openapi.md
- name: Coinbase API - Delete account
  x-api-slug: accountsaccount-id-delete
  description: "Removes user\u2019s account. In order to remove an account it can\u2019t
    be\n\n- Primary account\n- Account with non-zero balance\n- Fiat account\n- Vault
    with a pending withdrawal"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/accountsaccount-id-delete-openapi.md
- name: Coinbase API - Update account
  x-api-slug: accountsaccount-id-put
  description: "Modifies user\u2019s account name."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/accountsaccount-id-put-openapi.md
- name: Coinbase API - Show an account
  x-api-slug: accountsaccount-id-get
  description: "Show current user\u2019s account. To access user\u2019s primary account,
    primary keyword can be used instead of the account id in the URL."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/accountsaccount-id-get-openapi.md
- name: Coinbase API - Create account
  x-api-slug: accounts-post
  description: Creates a new account for user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/account/master/_listings/coinfabrik/accounts-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://blog.coinfabrik.com/feed/
- type: x-github
  url: https://github.com/CoinFabrik
- type: x-openapi
  url: https://raw.githubusercontent.com/CoinFabrik/coinbase-api-swagger/master/swagger.json
- type: x-api-gallery
  url: http://codefresh.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coinfabrik.stack.network
- type: x-blog
  url: https://blog.coinfabrik.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/coinfabrik
- type: x-twitter
  url: https://twitter.com/coinfabrik
- type: x-website
  url: https://www.coinfabrik.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---