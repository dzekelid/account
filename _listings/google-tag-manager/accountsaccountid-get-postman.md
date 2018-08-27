{
  "info": {
    "name": "Google Tag Manager API Get Account",
    "_postman_id": "7efb1282-f228-443e-9ff6-2d0eeed05ae9",
    "description": "Gets a GTM Account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "3cb18326-854c-4309-aa59-d5d763810e33",
          "name": "tagmanager.accounts.list",
          "request": {
            "url": "http://www.googleapis.com/tagmanager/v1/accounts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all GTM Accounts that a user has access to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f23718d-8153-46ec-a4d2-0456d6581717"
            }
          ]
        },
        {
          "id": "b4a83e24-d21c-4c77-9be1-ac5b10a3d17d",
          "name": "tagmanager.accounts.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tagmanager",
                "v1",
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
            "description": "Gets a GTM Account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42a19fab-5a90-459d-b2a5-162c0235ef2b"
            }
          ]
        }
      ]
    }
  ]
}