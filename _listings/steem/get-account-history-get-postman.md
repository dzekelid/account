{
  "info": {
    "name": "Steem Account history",
    "_postman_id": "c8994851-a2ee-45d9-a199-7623efa17221",
    "description": "Account history",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "e58944fc-a04b-40b9-a2fd-7d9967653d8b",
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
              "id": "7cc1dd57-9370-44fb-8099-c9132ea2da00"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "e6c61c8d-1c16-43f5-b32e-8c65b2e8878e",
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
              "id": "2b6fd8f3-b0ef-456a-baa2-b7c6762e9731"
            }
          ]
        },
        {
          "id": "6b16d21c-e6c7-41dd-979c-dc421c6ffed2",
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
              "id": "b7c52adc-7e31-4003-abf2-2ba1206a9f5f"
            }
          ]
        },
        {
          "id": "65d0188e-0b51-45e7-b63a-c4cf4c3f4c4e",
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
              "id": "ac6c54f8-4850-4ccd-b5a8-f0a7c8c1d3a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "bc80d398-23d0-4642-b53f-188ada8bce9e",
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
              "id": "a1c606ea-0e10-4a9d-8c0e-c51a5ba9f365"
            }
          ]
        },
        {
          "id": "e1f349a4-4e7e-47f9-a76b-67906f25ae64",
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
              "id": "68da13a4-c207-4ccc-9f8f-ca1d3f9f6769"
            }
          ]
        },
        {
          "id": "44a52913-a6d9-43a7-8c60-cd07a964a8fd",
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
              "id": "b0e6f138-a77a-4100-9799-1c4b53119a3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "47a2fb2a-f61c-4f62-94e9-274502950b64",
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
              "id": "03cc0789-b059-49ff-bbbc-08ce64a7359f"
            }
          ]
        },
        {
          "id": "8c8b77d5-4a24-4438-a648-370544c907f4",
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
              "id": "974445ba-3c70-494e-b2fc-de4c9bed6952"
            }
          ]
        }
      ]
    },
    {
      "name": "Verify",
      "item": [
        {
          "id": "5e5a9fad-7d01-44e8-bad2-eb8e195e1195",
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
              "id": "5db203be-59c0-455d-83a8-66d90d804eee"
            }
          ]
        }
      ]
    }
  ]
}