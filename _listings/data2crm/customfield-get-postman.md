{
  "info": {
    "name": "Data2CRM GET for CustomField",
    "_postman_id": "98060eeb-476a-4843-b79d-e473e8a76bed",
    "description": "Returns all custom field from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Custom",
      "item": [
        {
          "id": "40c10150-def3-424d-8164-19174646dd36",
          "name": "getCustomFieldCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/customField?entity=%7B%7D&filter=%7B%7D&label=%7B%7D&limit=%7B%7D&name=%7B%7D&offset=%7B%7D",
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
            "description": "Returns all custom field from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c29a26f-24d0-47d1-96f3-3acfb4337447"
            }
          ]
        }
      ]
    }
  ]
}