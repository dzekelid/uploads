---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Upload Attachment
  description: The upload attachment command is used to upload an attachment for sending.
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  attachments/upload/:
    get:
      summary: Upload Attachment
      description: The upload attachment command is used to upload an attachment for
        sending.
      operationId: getAttachmentsUpload
      x-api-path-slug: attachmentsupload-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: file
        description: The file name being uploaded
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Upload
  lists/upload-contacts:
    get:
      summary: Create Multiple Subscriber From CSV File
      description: Create Multiple Subscriber From CSV File
      operationId: getListsUploadContacts
      x-api-path-slug: listsuploadcontacts-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: title
        description: the title for the subscriber (Mr
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Upload
      - Contacts
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