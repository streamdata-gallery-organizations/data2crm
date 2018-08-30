---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM GET for Event
  description: Returns all events from the system
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
    put:
      summary: PUT for Account
      description: Update account information
      operationId: updateAccountEntity
      x-api-path-slug: accountaccount-id-put
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: body
        name: body
        description: Update account information
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
  /attachment:
    get:
      summary: GET for Attachment
      description: Returns all attachments from the system
      operationId: getAttachmentCollection
      x-api-path-slug: attachment-get
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
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
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
      - Attachments
    post:
      summary: POST for Attachment
      description: Add attachment into the system
      operationId: createAttachmentEntity
      x-api-path-slug: attachment-post
      parameters:
      - in: body
        name: body
        description: Add attachment into the system
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
      - Attachments
  /attachment/count:
    get:
      summary: COUNT for Attachment
      description: Count all attachments from the system
      operationId: getAttachmentCountCollection
      x-api-path-slug: attachmentcount-get
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
      - Attachments
      - Count
  /attachment/describe:
    get:
      summary: DESCRIBE for Attachment
      description: Returns describe for attachments
      operationId: getAttachmentDescribe
      x-api-path-slug: attachmentdescribe-get
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
      - Attachments
      - Describe
  /attachment/{attachment_id}:
    delete:
      summary: DELETE for Attachment
      description: Delete attachment information
      operationId: deleteAttachmentEntity
      x-api-path-slug: attachmentattachment-id-delete
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
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
      - Attachments
    get:
      summary: GET for Attachment
      description: Return attachment information
      operationId: getAttachmentEntity
      x-api-path-slug: attachmentattachment-id-get
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
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
      - Attachments
    put:
      summary: PUT for Attachment
      description: Update attachment information
      operationId: updateAttachmentEntity
      x-api-path-slug: attachmentattachment-id-put
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
      - in: body
        name: body
        description: Update attachment information
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
      - Attachments
  /call:
    get:
      summary: GET for Call
      description: Returns all calls from the system
      operationId: getCallCollection
      x-api-path-slug: call-get
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
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
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
      - Calls
    post:
      summary: POST for Call
      description: Add call into the system
      operationId: createCallEntity
      x-api-path-slug: call-post
      parameters:
      - in: body
        name: body
        description: Add call into the system
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
      - Calls
  /call/count:
    get:
      summary: COUNT for Call
      description: Count all calls from the system
      operationId: getCallCountCollection
      x-api-path-slug: callcount-get
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
      - Calls
      - Count
  /call/describe:
    get:
      summary: DESCRIBE for Call
      description: Returns describe for calls
      operationId: getCallDescribe
      x-api-path-slug: calldescribe-get
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
      - Calls
      - Describe
  /call/{call_id}:
    delete:
      summary: DELETE for Call
      description: Delete call information
      operationId: deleteCallEntity
      x-api-path-slug: callcall-id-delete
      parameters:
      - in: path
        name: call_id
        description: Call Identifier
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
      - Calls
    get:
      summary: GET for Call
      description: Return call information
      operationId: getCallEntity
      x-api-path-slug: callcall-id-get
      parameters:
      - in: path
        name: call_id
        description: Call Identifier
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
      - Calls
    put:
      summary: PUT for Call
      description: Update call information
      operationId: updateCallEntity
      x-api-path-slug: callcall-id-put
      parameters:
      - in: body
        name: body
        description: Update call information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: call_id
        description: Call Identifier
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
      - Calls
  /contact:
    get:
      summary: GET for Contact
      description: Returns all contacts from the system
      operationId: getContactCollection
      x-api-path-slug: contact-get
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
      - Contacts
    post:
      summary: POST for Contact
      description: Add contact into the system
      operationId: createContactEntity
      x-api-path-slug: contact-post
      parameters:
      - in: body
        name: body
        description: Add contact into the system
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
      - Contacts
  /contact/count:
    get:
      summary: COUNT for Contact
      description: Count all contacts from the system
      operationId: getContactCountCollection
      x-api-path-slug: contactcount-get
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
      - Contacts
      - Count
  /contact/describe:
    get:
      summary: DESCRIBE for Contact
      description: Returns describe for contacts
      operationId: getContactDescribe
      x-api-path-slug: contactdescribe-get
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
      - Contacts
      - Describe
  /contact/{contact_id}:
    delete:
      summary: DELETE for Contact
      description: Delete contact information
      operationId: deleteContactEntity
      x-api-path-slug: contactcontact-id-delete
      parameters:
      - in: path
        name: contact_id
        description: Contact Identifier
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
      - Contacts
    get:
      summary: GET for Contact
      description: Return contact information
      operationId: getContactEntity
      x-api-path-slug: contactcontact-id-get
      parameters:
      - in: path
        name: contact_id
        description: Contact Identifier
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
      - Contacts
    put:
      summary: PUT for Contact
      description: Update contact information
      operationId: updateContactEntity
      x-api-path-slug: contactcontact-id-put
      parameters:
      - in: body
        name: body
        description: Update contact information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contact_id
        description: Contact Identifier
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
      - Contacts
  /crm:
    get:
      summary: GET for Crm
      description: Returns all CRMs from the system
      operationId: getCrmCollection
      x-api-path-slug: crm-get
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
      - in: query
        name: type
        description: Type
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    post:
      summary: POST for Crm
      description: Add CRM into the systemWhat do I need to connect a CRM to Data2CRM.API?
      operationId: createCrmEntity
      x-api-path-slug: crm-post
      parameters:
      - in: body
        name: body
        description: Add CRM into the systemWhat do I need to connect a CRM to Data2CRM
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
  /crm/count:
    get:
      summary: COUNT for Crm
      description: Count all CRMs from the system
      operationId: getCrmCountCollection
      x-api-path-slug: crmcount-get
      parameters:
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Crm
      - Count
  /crm/{crm_id}:
    delete:
      summary: DELETE for Crm
      description: Delete CRM information
      operationId: deleteCrmEntity
      x-api-path-slug: crmcrm-id-delete
      parameters:
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    get:
      summary: GET for Crm
      description: Return CRM information
      operationId: getCrmEntity
      x-api-path-slug: crmcrm-id-get
      parameters:
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    put:
      summary: PUT for Crm
      description: Update CRM informationWhat do I need to connect a CRM to Data2CRM.API?
      operationId: updateCrmEntity
      x-api-path-slug: crmcrm-id-put
      parameters:
      - in: body
        name: body
        description: Update CRM informationWhat do I need to connect a CRM to Data2CRM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
  /customField:
    get:
      summary: GET for CustomField
      description: Returns all custom field from the system
      operationId: getCustomFieldCollection
      x-api-path-slug: customfield-get
      parameters:
      - in: query
        name: entity
        description: Entity
      - in: query
        name: filter
        description: Filter
      - in: query
        name: label
        description: Label
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: name
        description: Name
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
      - Custom
      - Fields
    post:
      summary: POST for CustomField
      description: Add custom field into the system
      operationId: createCustomFieldEntity
      x-api-path-slug: customfield-post
      parameters:
      - in: body
        name: body
        description: Add custom field into the system
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
      - Custom
      - Fields
  /customField/{custom_field_id}:
    delete:
      summary: DELETE for CustomField
      description: Delete custom field information
      operationId: deleteCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-delete
      parameters:
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
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
      - Custom
      - Fields
      - Custom
      - Field
    get:
      summary: GET for CustomField
      description: Return custom field information
      operationId: getCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-get
      parameters:
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
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
      - Custom
      - Fields
      - Custom
      - Field
    put:
      summary: PUT for CustomField
      description: Update custom field information
      operationId: updateCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-put
      parameters:
      - in: body
        name: body
        description: Update custom field information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
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
      - Custom
      - Fields
      - Custom
      - Field
  /email:
    get:
      summary: GET for Email
      description: Returns all emails from the system
      operationId: getEmailCollection
      x-api-path-slug: email-get
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
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
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
      - Emails
    post:
      summary: POST for Email
      description: Add email into the system
      operationId: createEmailEntity
      x-api-path-slug: email-post
      parameters:
      - in: body
        name: body
        description: Add email into the system
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
      - Emails
  /email/count:
    get:
      summary: COUNT for Email
      description: Count all emails from the system
      operationId: getEmailCountCollection
      x-api-path-slug: emailcount-get
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
      - Emails
      - Count
  /email/describe:
    get:
      summary: DESCRIBE for Email
      description: Returns describe for emails
      operationId: getEmailDescribe
      x-api-path-slug: emaildescribe-get
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
      - Emails
      - Describe
  /email/{email_id}:
    delete:
      summary: DELETE for Email
      description: Delete email information
      operationId: deleteEmailEntity
      x-api-path-slug: emailemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
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
      - Emails
    get:
      summary: GET for Email
      description: Return email information
      operationId: getEmailEntity
      x-api-path-slug: emailemail-id-get
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
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
      - Emails
    put:
      summary: PUT for Email
      description: Update email information
      operationId: updateEmailEntity
      x-api-path-slug: emailemail-id-put
      parameters:
      - in: body
        name: body
        description: Update email information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: email_id
        description: Email Identifier
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
      - Emails
  /event:
    get:
      summary: GET for Event
      description: Returns all events from the system
      operationId: getEventCollection
      x-api-path-slug: event-get
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
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
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
      - Events
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