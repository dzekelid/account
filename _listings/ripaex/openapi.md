swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/delegates/forging/getForgedByAccount:
    get:
      summary: Delegates Forging Get Forged By Account
      description: Get the amount of ripas forged by an account.
      operationId: delegates.getForgedByAccount
      x-api-path-slug: apidelegatesforginggetforgedbyaccount-get
      parameters:
      - in: query
        name: generatorPublicKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Forging
      - ""
      - Forged
      - Account