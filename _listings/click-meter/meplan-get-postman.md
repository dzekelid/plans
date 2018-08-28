{
  "info": {
    "name": "Click Meter Retrieve current account plan",
    "_postman_id": "fcca9767-c6a3-4155-bc87-00a2da387cf0",
    "description": "Retrieve current account plan.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Me",
      "item": [
        {
          "id": "29a540cf-ee46-4e04-9fa9-c9571f8bc3c9",
          "name": "getMe",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve current account data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c5a6fa6-5e94-4d07-b2da-530badd30950"
            }
          ]
        },
        {
          "id": "7aac11fd-1c79-47a5-b5e8-afe96c3707d4",
          "name": "getMePlan",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/me/plan",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve current account plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13479344-df5e-4ada-8774-62d0215f6ee0"
            }
          ]
        }
      ]
    }
  ]
}