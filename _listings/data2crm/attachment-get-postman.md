{
  "info": {
    "name": "Data2CRM GET for Attachment",
    "_postman_id": "fb661935-d7be-42a4-a1c3-89964f0d5c2a",
    "description": "Returns all attachments from the system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "c6f00972-bff8-4b3c-9a04-3a9bf0c0dd20",
          "name": "getAttachmentCollection",
          "request": {
            "url": "http://api.data2crm.com:80/v1/attachment?filter=%7B%7D&limit=%7B%7D&offset=%7B%7D&parent_id=%7B%7D&parent_type=%7B%7D",
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
            "description": "Returns all attachments from the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4396a172-3a9d-47f7-8580-6ebf8d47f149"
            }
          ]
        }
      ]
    }
  ]
}