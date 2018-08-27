{
  "info": {
    "name": "Click Meter Retrieve current account data",
    "_postman_id": "be341aef-5291-4905-ac5a-19c657776820",
    "description": "Retrieve current account data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "998b01e3-200a-419d-b83c-e3eca023b134",
          "name": "getAccount",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve current account data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b2d2257-a976-4112-8154-05e09b09ff7c"
            }
          ]
        }
      ]
    }
  ]
}