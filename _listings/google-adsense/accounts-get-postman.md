{
  "info": {
    "name": "Google Adsense API Get Accounts",
    "_postman_id": "a5742899-04fe-4ff9-ae9d-af9fc96f7d2c",
    "description": "List hosted accounts associated with this AdSense account by ad client id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Advertising",
      "item": [
        {
          "id": "0ca07097-cfb9-4994-a28a-da492d35391e",
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
              "id": "a8e253be-f245-4a57-90c2-29431c52c9dc"
            }
          ]
        }
      ]
    }
  ]
}