{
  "info": {
    "name": "Viddler  API Resellers GetSubaccounts",
    "_postman_id": "7862e681-d270-4593-871f-82d743e811ec",
    "description": "List all subaccounts under your account. Only applies to reseller accounts. Other accounts do not have access to this method.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "fbe6cbac-67bb-403d-8a61-39952d74de25",
          "name": "resellers-getsubaccounts",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.resellers.getSubaccounts?page=%7B%7D&per_page=%7B%7D&sessionid=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all subaccounts under your account. Only applies to reseller accounts. Other accounts do not have access to this method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16bedded-6dff-462f-895b-6a001d7c85a3"
            }
          ]
        }
      ]
    }
  ]
}