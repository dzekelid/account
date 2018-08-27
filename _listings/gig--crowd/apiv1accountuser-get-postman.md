{
  "info": {
    "name": "GIGANDCROWD Get Account User",
    "_postman_id": "7c0dc01f-e20d-49eb-8eb5-c34981a9aae1",
    "description": "Get account user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "53c653ec-bf4b-4b48-b856-179f26101411",
          "name": "getApiV1AccountUser",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/account/user",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get account user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1ed48ae-0f3c-452e-ab0a-351cf4d909cd"
            }
          ]
        }
      ]
    }
  ]
}