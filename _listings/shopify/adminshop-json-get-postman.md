{
  "info": {
    "name": "Shopify Get the configuration of the shop account",
    "_postman_id": "16ea1766-48b2-45da-b1f8-b9497c006eab",
    "description": "Get the configuration of the shop account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "f88228a9-7698-469d-99fc-6cbb328c4bdf",
          "name": "getAdminShop.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/shop.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get the configuration of the shop account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f94dca9-19e0-42c8-96f3-8e58ae0cb4f5"
            }
          ]
        }
      ]
    }
  ]
}