{
  "info": {
    "name": "Vzaar API Get Api Accounts Account",
    "_postman_id": "68daa563-5b74-4e37-85ee-85e19bdd8546",
    "description": "nnThis API call returns the details and rights for each vzaar subscription account type along with its relevant metadata. This will show the details of the packages available here: http://vzaar.com/pricingnn",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "dac00ebb-7cd8-4169-85a8-f19470cd4b2b",
          "name": "getApiAccountsAccount.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "vzaar.com",
              "path": [
                "api/accounts/:account.json"
              ],
              "query": [
                {
                  "key": "account is the vzaar account type. This is an integer.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "account",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "nnThis API call returns the details and rights for each vzaar subscription account type along with its relevant metadata. This will show the details of the packages available here: http://vzaar.com/pricingnn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32dfe076-19ba-4f70-8260-1ae26fd50374"
            }
          ]
        }
      ]
    }
  ]
}