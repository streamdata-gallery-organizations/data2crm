{
  "info": {
    "name": "Data2CRM GET for User",
    "_postman_id": "4e5d7b55-3c6e-47f3-8c29-f19e43cf1f1b",
    "description": "Returns all users from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "5407422d-c06c-409b-871c-0d0d846cea61",
          "name": "getUserCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/user?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API2CRM-CRMKEY",
                "value": "{}",
                "description": "CRM Key",
                "disabled": false
              },
              {
                "key": "X-API2CRM-DATA-ENABLE",
                "value": "{}",
                "description": "Data Enable",
                "disabled": false
              },
              {
                "key": "X-API2CRM-USERKEY",
                "value": "{}",
                "description": "User Key",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all users from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c63ce4e6-fe58-4647-9ec8-839e60498e2a"
            }
          ]
        }
      ]
    }
  ]
}