{
  "info": {
    "name": "Plentymarkets Get the revenue account configuration of a country",
    "_postman_id": "b9341ce0-50ac-4fb6-9714-95dec1e44656",
    "description": "Get the revenue account configuration of a country. The ID of the accounting location that the country is associated with as well as the ID of the country must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "d66fb3d3-b708-4829-bab2-a16407ffeffe",
          "name": "getRestAccountingLocationsExistingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/existing_accounts",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all unique posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2387c9f-3cd9-42e8-9506-49fcf9ee401f"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "1d2a0038-dc91-41bc-9f33-eb0c116b527d",
          "name": "getRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e787ce76-7fcb-4df1-b7ab-f9f00c3cd3cc"
            }
          ]
        },
        {
          "id": "a3a155f3-fb73-49e5-87af-7d2bb86ed584",
          "name": "getRestAccountingLocationsLocationAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all posting accounts by locationid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfa6df04-93bf-4039-811b-4c27d826401f"
            }
          ]
        },
        {
          "id": "339a75ae-c172-4858-b5f4-e6ff6d76c1af",
          "name": "getRestAccountingLocationsLocationTypeAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/:type/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all posting accounts by locationid and type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "584fe3ea-35fc-4538-929d-ff6272386dc1"
            }
          ]
        },
        {
          "id": "4319c33e-0416-4ce1-ab7d-486639d5d348",
          "name": "deleteRestAccountingLocationsAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/posting_accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete an posting account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c59230e-2bdb-4569-bd37-2246d07dd3e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Save",
      "item": [
        {
          "id": "9e313ee6-defa-4ccc-b2a7-3b1513d878e3",
          "name": "postRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Save posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f684a82d-1b4d-4904-a9e4-71a6ce55afd1"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "26ccab39-7556-4c60-8ec3-510d4a9ce044",
          "name": "getRestAccountingLocationsLocationDebtorAccountsMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/debtor_accounts/:mode"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists the debtor accounts of an accounting location by mode. The ID of the accounting location and the mode have to be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67573173-ac71-4e7d-8132-0d72e79c817b"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "13adadfb-4638-4559-bee0-c54ad34d0668",
          "name": "getRestAccounts",
          "request": {
            "url": "http://example.com/rest/accounts?createdAt=%7B%7D&updatedAt=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16213d59-19ab-459f-b76c-c8f5c41bd8e7"
            }
          ]
        },
        {
          "id": "0460d47c-cacb-4385-a763-79a51252698a",
          "name": "getRestAccountsContactsContactBanks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/banks"
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists bank accounts of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "311d0dc4-d60b-4827-8ef6-599e90199af4"
            }
          ]
        },
        {
          "id": "6c4bde4c-6e1b-45eb-91c4-02d1bc68408d",
          "name": "getRestItemsSalesPricesAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/accounts"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all activated referrer accounts of a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbd2036b-6559-40e6-975e-974a45483db7"
            }
          ]
        },
        {
          "id": "2a6a0d90-39a3-4d7a-b423-9cfc42ce607e",
          "name": "getRestAccountingLocationsRevenueAccountConfigurations",
          "request": {
            "url": "http://example.com/rest/accounting/locations/revenue_account_configurations?itemsPerPage=%7B%7D&page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists revenue account configurations of a system. The revenue accounts are returned as paginated result. By default 50 revenue accounts are on one page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bdf8943-e7be-45c6-ad4b-a23a235c91ae"
            }
          ]
        }
      ]
    },
    {
      "name": "EBICS",
      "item": [
        {
          "id": "e161ab01-b028-40cb-aa50-88d46da605c6",
          "name": "getRestPaymentsMethodsEbics",
          "request": {
            "url": "http://example.com/rest/payments/methods/ebics",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get ebics accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d677cb24-f1db-4cd6-a8ff-51e37352d8c1"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "744f025b-0a95-4585-85a7-267a89f212fd",
          "name": "getRestAccountingLocationsAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/posting_accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets posting account by the unique id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "532d9e5f-45f0-46b2-ab5c-1203444ec19f"
            }
          ]
        }
      ]
    },
    {
      "name": "Revenue",
      "item": [
        {
          "id": "b5518ca7-458d-4274-88ee-6a5528bb34e4",
          "name": "getRestAccountingLocationsLocationCountriesCountryRevenueAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/countries/:countryId/revenue_accounts"
              ],
              "variable": [
                {
                  "id": "countryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the revenue account configuration of a country. The ID of the accounting location that the country is associated with as well as the ID of the country must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95c1354e-2ee8-49fa-9cf5-e5d3019d0ee7"
            }
          ]
        }
      ]
    }
  ]
}