{
  "info": {
    "name": "Google Tag Manager API Get Accounts",
    "_postman_id": "93c23a81-48a2-4612-9d9e-d3ef2de8d1e0",
    "description": "Lists all GTM Accounts that a user has access to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "a36d93cf-3acf-49c9-b2d8-6d69995c309a",
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
              "id": "a6442b4f-54b1-47c4-9db0-ef4482477593"
            }
          ]
        }
      ]
    }
  ]
}