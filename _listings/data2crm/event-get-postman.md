{
  "info": {
    "name": "Data2CRM GET for Event",
    "_postman_id": "218ea2de-d090-47fc-b806-26d74fbcc8be",
    "description": "Returns all events from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "66933d5e-47f5-4857-b4df-20eae0dde27b",
          "name": "getEventCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/event?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D&parent_id=%7B%7D&parent_type=%7B%7D",
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
            "description": "Returns all events from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6154cae9-6523-4aa2-8e7a-056520e2405f"
            }
          ]
        }
      ]
    }
  ]
}