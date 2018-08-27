swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 1
info:
  title: Capital One DevExchange
  description: nessie-is-capital-ones-hackathon-api-that-gives-you-access-to-a-multitude-of-real-publicfacing-data--such-as-atm-and-bank-branch-locations--along-with-mock-customer-account-data--use-http-requests-to-set-up-peertopeer-transactions-simulate-a-weekly-paycheck-or-even-schedule-bills-for-customers-this-is-all-structured-in-a-way-that-resembles-how-we-actually-run-things-here-at-capital-one-
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /merchants/{id}/accounts/{accountId}/purchases:
    get:
      summary: Get all purchases by account and merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidaccountsaccountidpurchases-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account associated with all the purchases
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Accounts
      - Account
      - Purchases