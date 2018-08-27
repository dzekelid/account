{
  "info": {
    "name": "Steem get_witness_by_account",
    "_postman_id": "9c5562a6-2c7d-4025-a2ea-335f8b89e76f",
    "description": "get_witness_by_account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "7d3387d6-b663-4934-af24-7e436f46cb8f",
          "name": "get-number-of-accounts-from-steem",
          "request": {
            "url": "http://api.steemjs.com/get_account_count",
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
            "description": "Get Number of Accounts from Steem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8c9cb13-455a-46ea-a58b-4313a352b352"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "b43287fb-d197-4767-a4fb-2f833e9070ab",
          "name": "lookup-witness-accounts-regex-search",
          "request": {
            "url": "http://api.steemjs.com/lookup_witness_accounts?limit=%7B%7D&lowerBoundName=%7B%7D",
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
            "description": "lookup_witness_accounts regex search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa687ff3-8652-4fcc-9ea4-1cd46d57dd9b"
            }
          ]
        },
        {
          "id": "f933b817-5fa4-48af-8bd2-2542c53e1978",
          "name": "lookup-accounts-regex-search",
          "request": {
            "url": "http://api.steemjs.com/lookup_accounts?limit=%7B%7D&lowerBoundName=%7B%7D",
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
            "description": "lookup_accounts regex search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb953bc8-7620-4f29-b6d7-91052a8f243f"
            }
          ]
        },
        {
          "id": "1b2f7d2b-9421-4fc2-863f-259ca25e7bce",
          "name": "lookup-account-names-example-of-accountnames-goodkarma-fabien",
          "request": {
            "url": "http://api.steemjs.com/lookup_account_names?accountNames=%7B%7D",
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
            "description": "lookup_account_names example of accountNames [\"good-karma\", \"fabien\"]"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "756bdc0b-9598-4b25-9977-01bc550ded21"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "eb7b8c8d-8fcb-4532-9c67-468bc43e82d7",
          "name": "get-witness-by-account",
          "request": {
            "url": "http://api.steemjs.com/get_witness_by_account?accountName=%7B%7D",
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
            "description": "get_witness_by_account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01dcb3c2-4497-4ba9-89a6-bdf795bdb463"
            }
          ]
        },
        {
          "id": "86ae1459-6877-4b68-a8f0-bbad8cd3fb7b",
          "name": "get-account-votes",
          "request": {
            "url": "http://api.steemjs.com/get_account_votes?voter=%7B%7D",
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
            "description": "get_account_votes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "370e1436-c0f3-41b9-bc3a-3d8631f3a940"
            }
          ]
        },
        {
          "id": "2e462904-563e-424e-b231-d79fb8c92d83",
          "name": "get-account-bandwidth",
          "request": {
            "url": "http://api.steemjs.com/get_account_bandwidth?account=%7B%7D&bandwidthType=%7B%7D",
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
            "description": "get_account_bandwidth"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6db46af1-1e8d-44a6-9861-ec6ed8d0c083"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "7c9ab45a-283d-4e1c-b301-de7c76d77ad2",
          "name": "account-history",
          "request": {
            "url": "http://api.steemjs.com/get_account_history?account=%7B%7D&from=%7B%7D&limit=%7B%7D",
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
            "description": "Account history"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2d053f9-b613-47b0-b94a-660208e99e7f"
            }
          ]
        },
        {
          "id": "b9308432-20b4-427d-9781-9f2230c3b5f3",
          "name": "get-accounts-from-steem",
          "request": {
            "url": "http://api.steemjs.com/get_accounts?names=%5B%7B%7D%5D",
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
            "description": "Get Accounts from Steem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a1fb015-99a7-4fde-9ced-e31684a4ae1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Verify",
      "item": [
        {
          "id": "d492bc3c-58d3-45a5-86a9-f64c7094cba6",
          "name": "verify-account-authority",
          "request": {
            "url": "http://api.steemjs.com/verify_account_authority?nameOrId=%7B%7D&signers=%7B%7D",
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
            "description": "verify_account_authority"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0669c56a-096a-4456-9bef-06db3b8d24af"
            }
          ]
        }
      ]
    }
  ]
}