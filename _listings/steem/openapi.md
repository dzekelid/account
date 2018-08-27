swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /verify_account_authority:
    get:
      summary: verify_account_authority
      description: verify_account_authority
      operationId: verify-account-authority
      x-api-path-slug: verify-account-authority-get
      parameters:
      - in: query
        name: nameOrId
        description: nameOrId
      - in: query
        name: signers
        description: signers
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Account
      - Authority
  /get_account_bandwidth:
    get:
      summary: get_account_bandwidth
      description: get_account_bandwidth
      operationId: get-account-bandwidth
      x-api-path-slug: get-account-bandwidth-get
      parameters:
      - in: query
        name: account
        description: account name
      - in: query
        name: bandwidthType
        description: bandwidthType
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Bandwidth
  /lookup_account_names:
    get:
      summary: lookup_account_names
      description: lookup_account_names example of accountNames ["good-karma", "fabien"]
      operationId: lookup-account-names-example-of-accountnames-goodkarma-fabien
      x-api-path-slug: lookup-account-names-get
      parameters:
      - in: query
        name: accountNames
        description: accountNames [good-karma, fabien]
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Account
      - Names
  /get_accounts:
    get:
      summary: Account
      description: Get Accounts from Steem
      operationId: get-accounts-from-steem
      x-api-path-slug: get-accounts-get
      parameters:
      - in: query
        name: names[]
        description: name of account
      responses:
        200:
          description: OK
      tags:
      - Account
  /get_account_history:
    get:
      summary: Account history
      description: Account history
      operationId: account-history
      x-api-path-slug: get-account-history-get
      parameters:
      - in: query
        name: account
        description: name of account
      - in: query
        name: from
        description: from
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Account
      - History
  /get_account_votes:
    get:
      summary: get_account_votes
      description: get_account_votes
      operationId: get-account-votes
      x-api-path-slug: get-account-votes-get
      parameters:
      - in: query
        name: voter
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Account
      - Votes
  /get_witness_by_account:
    get:
      summary: get_witness_by_account
      description: get_witness_by_account
      operationId: get-witness-by-account
      x-api-path-slug: get-witness-by-account-get
      parameters:
      - in: query
        name: accountName
        description: witness account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - By
      - Account