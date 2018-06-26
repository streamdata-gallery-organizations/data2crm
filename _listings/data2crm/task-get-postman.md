{
  "info": {
    "name": "Data2CRM GET for Task",
    "_postman_id": "f738c3ba-a6c2-4c4c-a0de-51e2dc78e338",
    "description": "Returns all tasks from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tasks",
      "item": [
        {
          "id": "a834ab0c-a1b9-48cc-b22e-9319ff4dd7b0",
          "name": "getTaskCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/task?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D",
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
            "description": "Returns all tasks from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b4c22ca-3167-469e-be83-4fefe9cfca09"
            }
          ]
        }
      ]
    }
  ]
}