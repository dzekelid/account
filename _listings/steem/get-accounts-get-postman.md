{
  "info": {
    "name": "Steem Account",
    "_postman_id": "1498823e-cd20-4d2a-a1c5-6276fada3059",
    "description": "Get Accounts from Steem",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "b0c70f77-5cad-45e1-a145-9c5e1c70cc3e",
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
              "id": "29dfa2cf-7361-466f-b8ff-db7fd54f6fbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "8ff160b8-7b8d-45cc-acba-8df7b0da4701",
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
              "id": "b65ae87f-956a-4ea5-9523-4a137e8acf4c"
            }
          ]
        },
        {
          "id": "19c2cc26-3e69-4954-9b34-00724a59576f",
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
              "id": "5daac106-e5af-4b62-898f-44ea6fef4d58"
            }
          ]
        },
        {
          "id": "a113cc96-1281-443d-a91b-48be2eb01723",
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
              "id": "6cd064fa-5502-4d08-a60f-ed5eaef2b306"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "bb794d70-77bb-437d-8adb-fa926dc40490",
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
              "id": "e6468fd6-6c81-4efe-92a8-14bef053911f"
            }
          ]
        },
        {
          "id": "db6e7f4e-b123-47b7-994d-bf6b6af4b0fb",
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
              "id": "5d48e0c6-1be6-4253-b0ed-9cb989acaf9b"
            }
          ]
        },
        {
          "id": "e69005e8-331d-4063-b331-4e6b96dcf82d",
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
              "id": "e65ecbac-1a76-4589-80a7-5b99e65a944a"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "6d95ad6e-1829-4be8-99ad-91ca0f437be0",
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
              "id": "5f1b5616-5bdf-4cda-9fe9-51b034566647"
            }
          ]
        },
        {
          "id": "27c49136-cfbd-4b51-9abe-35513e7da310",
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
              "id": "5414ca7c-c33c-402c-b324-17d77329f08e"
            }
          ]
        }
      ]
    },
    {
      "name": "Verify",
      "item": [
        {
          "id": "aa9d438e-27a0-4035-9725-d280f2adf5bd",
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
              "id": "34aa96d4-6201-41ba-bb34-02a6a3fc23dd"
            }
          ]
        }
      ]
    }
  ]
}