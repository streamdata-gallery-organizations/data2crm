{
  "info": {
    "name": "Data2CRM GET for Call",
    "_postman_id": "724a6824-e243-4572-a8ee-6333314dc19b",
    "description": "Returns all calls from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calls",
      "item": [
        {
          "id": "d592ad31-bcb9-47b5-bba0-60f0527ed969",
          "name": "getCallCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/call?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D&parent_id=%7B%7D&parent_type=%7B%7D",
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
            "description": "Returns all calls from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bad45f5-b241-4ee3-8956-11b5af196960"
            }
          ]
        }
      ]
    }
  ]
}