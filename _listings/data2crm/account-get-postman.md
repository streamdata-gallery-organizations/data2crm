{
  "info": {
    "name": "Data2CRM GET for Account",
    "_postman_id": "c658d160-f837-4c12-98d9-8e0a3213929a",
    "description": "Returns all accounts from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "3f202c38-08d6-488c-9a82-cc0dabeceb0c",
          "name": "getAccountCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/account?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D",
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
            "description": "Returns all accounts from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18d87c5-2098-4944-b1f6-ba25689cea65"
            }
          ]
        }
      ]
    }
  ]
}