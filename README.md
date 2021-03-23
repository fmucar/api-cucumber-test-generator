# api-cucumber-test-generator




Sample input format

```json
{
  "CurrencyApi": {
    "description": "Conversion API",
    "environments": [
      {
        "name": "dev",
        "protocol": "http",
        "host": "data.fixer.io",
        "port": 80
      },
      {
        "name": "ci",
        "protocol": "http",
        "host": "data.fixer.io",
        "port": 80
      }
    ],
    "scenarios": [
      {
        "scenarioNumber": 1,
        "groupName": "application",
        "requestMethod": "GET",
        "contextPath": "/api/convert",
        "description": "testing adding customer",
        "consumes": "application/json",
        "produces": "application/json",
        "queryParams": {
          "access_key": "ACCESS_KEY",
          "from": "GBP",
          "to": "USD",
          "amount": "1"
        },
        "hasRequestBody": "true",
        "hasResponseBody": "true",
        "responseStatus": 200
      }
    ]
  }
}

```