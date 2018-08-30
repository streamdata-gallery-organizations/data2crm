{
  "info": {
    "name": "Data2CRM GET for Email",
    "_postman_id": "7efd1ca0-5dd4-443f-9b87-80a4a74bdb78",
    "description": "Returns all emails from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Emails",
      "item": [
        {
          "id": "12ae0677-2d01-49dd-8f63-002b6e6be5c3",
          "name": "getEmailCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/email?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D&parent_id=%7B%7D&parent_type=%7B%7D",
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
            "description": "Returns all emails from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b9e7c28-706e-4532-909c-660f3165973f"
            }
          ]
        }
      ]
    }
  ]
}