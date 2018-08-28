{
  "info": {
    "name": "Stripe Get Plans",
    "_postman_id": "1aeee592-9483-4893-bc3a-64978dbd8c4c",
    "description": "Returns a list of your plans.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "plans",
      "item": [
        {
          "id": "e4233a09-17ac-4bf0-bad9-622ecee96e73",
          "name": "getPlans",
          "request": {
            "url": "http://api.stripe.com/v1/plans?created=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of your plans"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be252c64-bede-4fe7-bf43-e50492923126"
            }
          ]
        }
      ]
    }
  ]
}