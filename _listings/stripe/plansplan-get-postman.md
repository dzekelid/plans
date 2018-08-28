{
  "info": {
    "name": "Stripe Get Plans Plan",
    "_postman_id": "cd5e2e6f-e664-466b-8b2c-1f3c2fd3ea7d",
    "description": "Retrieves the plan with the given ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "plans",
      "item": [
        {
          "id": "86c1f730-d194-4b50-a018-69773e259a6f",
          "name": "getPlansPlan",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "plans/:plan"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "plan",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the plan with the given ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29a5a757-e310-4cf1-9d96-6a73d06c1b41"
            }
          ]
        }
      ]
    }
  ]
}