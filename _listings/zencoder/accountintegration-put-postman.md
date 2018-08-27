{
  "info": {
    "name": "Zencoder API Integration Mode",
    "_postman_id": "3db9a84d-0350-44b3-b66f-860e2b1153f8",
    "description": "Integration Mode",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "eda2ec29-c566-49f1-a87a-b45b53e843d7",
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
              "id": "3c5599fb-ca4d-4584-befc-c494f5cb8f48"
            }
          ]
        },
        {
          "id": "242581e9-f6e2-45d2-ba59-46039981fd21",
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
              "id": "39bc1790-3402-493a-b6a6-2861a5703b48"
            }
          ]
        },
        {
          "id": "7bb0a766-c8c9-4d96-ab67-4998fb51c9ec",
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
              "id": "6deaa981-bd98-44ff-8b0e-ac27a020327f"
            }
          ]
        }
      ]
    }
  ]
}