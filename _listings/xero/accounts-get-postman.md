{
  "info": {
    "name": "Clarity Accounting Get Accounts",
    "_postman_id": "d8351bc7-b4ff-46a9-bce1-6213705227a5",
    "description": "Retrieve the chart of accounts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "c523b378-ca23-46c0-accd-be65b547a168",
          "name": "getAccounts",
          "request": {
            "url": "http://api.xero.com/api.xro/2.0/Accounts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the chart of accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5456a74b-3e98-4f47-8d25-18ef6c8a2877"
            }
          ]
        }
      ]
    }
  ]
}