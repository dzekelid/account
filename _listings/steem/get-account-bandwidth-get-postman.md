{
  "info": {
    "name": "Steem get_account_bandwidth",
    "_postman_id": "71ce93e4-ab3e-4b19-8dbc-6cbd6f88c3d3",
    "description": "get_account_bandwidth",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "79c46708-7341-4e5a-ad84-929b81ecbcdb",
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
              "id": "ff08d521-3435-41bf-a1c8-410be028658d"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "84dec5d6-2ec9-451e-9bdb-9612fed4960e",
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
              "id": "3d7a4cc1-15a9-478c-8810-ac0dbf66bc2c"
            }
          ]
        },
        {
          "id": "9bab3c6f-0373-46e1-80d8-22632d3ddf9f",
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
              "id": "3d07b5da-7543-459e-bfcb-1d12207daf0e"
            }
          ]
        },
        {
          "id": "a9293e4b-ce11-48a9-9107-356dd7878270",
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
              "id": "34ffc68b-9c0c-4ed0-b366-6baa5ef6da20"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "511573c3-4170-4cc0-8501-54f9110897d4",
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
              "id": "21a721d5-c482-4ff9-a717-33c873c7dcc3"
            }
          ]
        },
        {
          "id": "fe33b32f-38fe-4ab8-a29c-711569e10d8d",
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
              "id": "d554e80d-b204-4c39-a0b5-71c9986288a7"
            }
          ]
        },
        {
          "id": "7bc78b9c-da58-45c3-bd27-39cfe229d126",
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
              "id": "f9517248-477a-4921-bb89-613ce1670a38"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "377ac6fd-90c0-4a56-a726-dc5db523a0e8",
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
              "id": "1cf31f60-f21c-4933-889a-ad95bbcfe3fc"
            }
          ]
        },
        {
          "id": "4dd58417-3ad2-44cb-8968-da93b72330c1",
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
              "id": "b0fc6282-d339-444d-83d8-31ab0fc3e0c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Verify",
      "item": [
        {
          "id": "9a334133-227a-4aeb-99c6-ae8445321277",
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
              "id": "e1d24d17-49f4-4002-960f-267002f53f2c"
            }
          ]
        }
      ]
    }
  ]
}