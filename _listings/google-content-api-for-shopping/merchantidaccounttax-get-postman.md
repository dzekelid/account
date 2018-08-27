{
  "info": {
    "name": "Google Content API for Shopping API Get Account Taxes",
    "_postman_id": "5374e391-561f-4370-85a9-e7d7ff8fd42f",
    "description": "Lists the tax settings of the sub-accounts in your Merchant Center account. This method can only be called for multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "account",
      "item": [
        {
          "id": "fd6e760a-c5eb-4a01-8c8e-0add620c81cc",
          "name": "content.accounttax.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/accounttax"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "merchantId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tax settings of the sub-accounts in your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d677ae43-9863-4740-bf61-83ef23964a38"
            }
          ]
        }
      ]
    }
  ]
}