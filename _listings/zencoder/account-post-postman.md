{
  "info": {
    "name": "Zencoder API Create an Account",
    "_postman_id": "2ff1e74b-22d3-4d32-9ffc-4c1e7b11636a",
    "description": "Create an Account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "d7288193-b7c5-4a4b-aacf-a6a2b3a6ae14",
          "name": "getAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f296e74-25e9-4d74-93d1-ab3bba89c2ff"
            }
          ]
        },
        {
          "id": "6f061a1d-8585-4ffa-8f37-d95a534bb3c3",
          "name": "postAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?email=%7B%7D&password=%7B%7D&password_confirmation=%7B%7D&terms_of_service=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c104c817-6569-49cf-81ad-b708db648cee"
            }
          ]
        }
      ]
    }
  ]
}