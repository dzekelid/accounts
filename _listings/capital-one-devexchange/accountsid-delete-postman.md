{
  "info": {
    "name": "Capital One DevExchange Delete a specific existing account",
    "_postman_id": "b655d6dc-0434-48b2-a623-9a0c3534db31",
    "description": "Deletes the specific account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "15136fbe-1daa-4d05-b4bd-88fb1eefa826",
          "name": "deletes-the-specific-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specific account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "979d2cfb-c869-4dde-a1ab-ae13f989cde3"
            }
          ]
        }
      ]
    }
  ]
}