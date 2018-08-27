{
  "info": {
    "name": "Plentymarkets List revenue account configurations",
    "_postman_id": "dd8c59ae-d6f0-4e51-b98e-a18e517ad6b5",
    "description": "Lists revenue account configurations of a system. The revenue accounts are returned as paginated result. By default 50 revenue accounts are on one page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "bfbfb7d9-59e8-4b4d-a9d6-8caaf0034846",
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
              "id": "aed66988-d103-4dde-9d65-2d41237f325b"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "8d56fff0-a10e-4706-bc54-c53727645e04",
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
              "id": "189d3e4c-0985-419f-87e0-4d3ef7103f36"
            }
          ]
        },
        {
          "id": "0a513526-0995-460d-9703-207ddb23b9cc",
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
              "id": "f47c64b4-4c1c-457c-8094-22a0b8a0aa07"
            }
          ]
        },
        {
          "id": "58949f0f-0d85-4974-b430-3af41c2483fc",
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
              "id": "045ea80e-5909-409a-bc17-b93e6ff29d94"
            }
          ]
        },
        {
          "id": "4e8258c3-7396-4fbf-9595-0d12a1373009",
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
              "id": "f62b8c4a-6489-4ac6-b185-77d760c77fcc"
            }
          ]
        }
      ]
    },
    {
      "name": "Save",
      "item": [
        {
          "id": "4b060fe8-92ea-43d5-aa3b-ef7af5b54211",
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
              "id": "57fe306b-ced7-4aa0-b621-3a7e1553aeb8"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "38d7e02f-90ab-4aba-b3da-31c68f94d4c9",
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
              "id": "1f15be25-69ef-4b2c-a869-81d654049372"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "4fb48483-b4ec-4626-9e84-410806c5d2b0",
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
              "id": "be59d1ed-83ec-45ce-92d0-e1c97cd2c196"
            }
          ]
        },
        {
          "id": "14fa6cc2-43a5-4635-9c00-59d0296163e7",
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
              "id": "419b7581-2772-4e51-b1d8-7a540c509ac2"
            }
          ]
        },
        {
          "id": "b3e3e97c-6214-4fab-b2ef-b8de45d912ff",
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
              "id": "5ad874ca-72fc-4d46-90a8-b0d5bbf86c8c"
            }
          ]
        },
        {
          "id": "6bc79c9d-e0fe-4126-b1eb-310b90797d1a",
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
              "id": "6a372e2b-5098-44c1-8fb8-b72d8b419a07"
            }
          ]
        }
      ]
    },
    {
      "name": "EBICS",
      "item": [
        {
          "id": "f4903821-0a07-4131-b813-cd04a53e6c07",
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
              "id": "99693d8d-67c4-41f4-bdb8-b01e48946644"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "30063aaa-34c8-4bf3-ba77-76c6d2d1c2c2",
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
              "id": "e485e68c-6178-4d99-b8bd-ce8b15306d29"
            }
          ]
        }
      ]
    }
  ]
}