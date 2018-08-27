{
  "info": {
    "name": "Steem lookup_account_names",
    "_postman_id": "e331147e-8a02-4855-8bc0-f7e0f7f3d063",
    "description": "lookup_account_names example of accountNames [\"good-karma\", \"fabien\"]",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Number",
      "item": [
        {
          "id": "82599718-a858-4f0e-8c72-14e6ffe6c0e3",
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
              "id": "344d7206-2d8b-469d-8fdd-d11095e4f4f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "d7fb2e02-5995-4953-9a63-8084353689f4",
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
              "id": "1d06ee51-b819-42d9-8885-66ff7bd372a3"
            }
          ]
        },
        {
          "id": "042552d6-e07d-4dd5-a3de-86b7211b7d16",
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
              "id": "d860f4b9-a5ae-4ec6-a1ce-888fa18221f8"
            }
          ]
        },
        {
          "id": "c94d8b6c-4050-4e1b-8833-c2bafa872d2d",
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
              "id": "ac3e9ba4-ab33-4143-9dce-df8d86cb4c2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "240ac2b5-c1b9-435b-848a-3e2d6b9a973e",
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
              "id": "05ef0e19-6880-48f9-b787-e03748fda612"
            }
          ]
        },
        {
          "id": "8008ff08-8924-40b2-adb3-77e9d3d871d0",
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
              "id": "07662c64-0271-4b31-bc8d-47d3b33304fe"
            }
          ]
        },
        {
          "id": "7080bf7f-fdb0-449a-a04e-6e5e58494b7c",
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
              "id": "e431d0c3-b7d8-4667-8e10-3d85998aad03"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "a8bbee1c-3402-4f86-a562-c2a55e68dd9c",
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
              "id": "67214673-02d6-4d66-a6ce-b748cc07001d"
            }
          ]
        },
        {
          "id": "c0bbf49b-cb85-403f-8118-27f2bdc657b6",
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
              "id": "342bb8dd-0edd-4704-b466-83c5221aac68"
            }
          ]
        }
      ]
    },
    {
      "name": "Verify",
      "item": [
        {
          "id": "cfb918db-df5f-4336-9779-49552dbc9e73",
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
              "id": "988f92f8-7980-4380-a107-7c158705a846"
            }
          ]
        }
      ]
    }
  ]
}