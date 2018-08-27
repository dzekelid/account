{
  "info": {
    "name": "Zencoder API Integration Mode - Live",
    "_postman_id": "195bb4c1-4faa-423a-8281-a8ebe2e0205e",
    "description": "Integration Mode - Live",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "01fe2200-ac39-4d36-a7fb-68ecef89f39c",
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
              "id": "7b7b3ace-863c-406e-af69-0d297dd5cf2a"
            }
          ]
        },
        {
          "id": "d8e880f2-a37b-4658-ab99-4162ba4b981f",
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
              "id": "2ada8b8d-c0c3-4b14-9828-e7eeeb3b4c87"
            }
          ]
        },
        {
          "id": "0d6e2a40-4c17-4869-bbd0-2c0dc2d12d05",
          "name": "putAccountIntegration",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/integration?api_key=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8301567a-b9b4-4047-9e3e-85c9bd566db6"
            }
          ]
        },
        {
          "id": "e2b9702a-2ffc-4acc-beb2-cb1978fab325",
          "name": "putAccountLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/live",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode - Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba4d074a-96c4-4e38-90b0-9f7a68b2abd4"
            }
          ]
        }
      ]
    }
  ]
}