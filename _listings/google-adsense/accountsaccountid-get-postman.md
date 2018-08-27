{
  "info": {
    "name": "Google Adsense API Get Account",
    "_postman_id": "d1688cf2-ac71-48c3-8db1-1eadd45271c0",
    "description": "Get information about the selected associated AdSense account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Advertising",
      "item": [
        {
          "id": "b35b44d0-17ff-4226-a066-7d7af36eefc5",
          "name": "adsensehost.accounts.list",
          "request": {
            "url": "http://example.com/api/accounts?filterAdClientId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List hosted accounts associated with this AdSense account by ad client id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70e7b45a-4969-4c31-bf02-864948f4b5de"
            }
          ]
        },
        {
          "id": "769e2b8f-ab5b-40c5-b162-738889108733",
          "name": "adsensehost.accounts.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "accounts/:accountId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about the selected associated AdSense account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "525242d3-d578-43f1-a602-03bc739ff477"
            }
          ]
        }
      ]
    }
  ]
}