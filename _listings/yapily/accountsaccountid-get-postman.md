{
  "info": {
    "name": "Yapily Get account",
    "_postman_id": "4686aed5-7c17-49ea-a965-2cac110d1ddf",
    "description": "Get account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "fb2ffc8e-be35-47a1-aab0-50d9e90709ef",
          "name": "getAccountsUsingGET",
          "request": {
            "url": "http://api.yapily.com:443/accounts",
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b87da3ba-96f9-425c-96e3-fccdb13a42e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "abc7ec98-7b10-4df1-a591-70a43dbea347",
          "name": "getAccountUsingGET",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.yapily.com",
              "path": [
                "accounts/:accountId"
              ],
              "port": "443",
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d311590c-27e1-4ea5-bbd7-7d715e88710e"
            }
          ]
        }
      ]
    }
  ]
}