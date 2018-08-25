{
  "info": {
    "name": "Yapily Get accounts",
    "_postman_id": "9661bb95-fbbc-42d2-b830-a75c6d887a27",
    "description": "Get accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "937bc691-4e63-4145-89a4-102c1a7db0d3",
          "name": "getAccountsUsingGET",
          "request": {
            "url": "http://api.yapily.com:443/accounts",
            "method": "GET",
            "header": [
              {
                "key": "consent",
                "value": "{}",
                "description": "Consent Token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98f143c4-7abc-4cbf-a184-a40c6a1f376e"
            }
          ]
        }
      ]
    }
  ]
}