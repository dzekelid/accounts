{
  "info": {
    "name": "Dezrez Get all accounts paginated",
    "_postman_id": "cdd70b25-fc0e-456b-9c48-2790713a6a73",
    "description": "Get all accounts paginated.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "e8034c80-a2b4-4c52-a5aa-30169e687aaf",
          "name": "Account_GetAllBypageSizeBypageNumber",
          "request": {
            "url": "http://api.dezrez.com/api/account/all?pageNumber=%7B%7D&pageSize=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Get all accounts paginated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1a53094-e0b1-4a79-af20-5ae6705f7a65"
            }
          ]
        }
      ]
    }
  ]
}