---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM GET for Account
  description: Return account information
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: GET for Account
      description: Returns all accounts from the system
      operationId: getAccountCollection
      x-api-path-slug: account-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: POST for Account
      description: Add account into the system
      operationId: createAccountEntity
      x-api-path-slug: account-post
      parameters:
      - in: body
        name: body
        description: Add account into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /account/count:
    get:
      summary: COUNT for Account
      description: Count all accounts from the system
      operationId: getAccountCountCollection
      x-api-path-slug: accountcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Count
  /account/describe:
    get:
      summary: DESCRIBE for Account
      description: Returns describe for accounts
      operationId: getAccountDescribe
      x-api-path-slug: accountdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Describe
  /account/{account_id}:
    delete:
      summary: DELETE for Account
      description: Delete account information
      operationId: deleteAccountEntity
      x-api-path-slug: accountaccount-id-delete
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    get:
      summary: GET for Account
      description: Return account information
      operationId: getAccountEntity
      x-api-path-slug: accountaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---