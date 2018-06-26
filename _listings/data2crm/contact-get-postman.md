{
  "info": {
    "name": "Data2CRM GET for Contact",
    "_postman_id": "e611767c-356e-47d6-87ac-9499ea795e46",
    "description": "Returns all contacts from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "0c0a0dcb-424b-4de0-b401-6e3468af292f",
          "name": "getContactCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/contact?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D",
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
            "description": "Returns all contacts from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "013bd0fe-59e2-44a9-9504-d60ede91c138"
            }
          ]
        }
      ]
    }
  ]
}