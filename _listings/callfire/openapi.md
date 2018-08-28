swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/lists/upload:
    post:
      summary: Create contact list from file
      description: Creates a contact list to be used with campaigns through uploading
        a .csv file. Returns the id of created list
      operationId: createContactListFromFile
      x-api-path-slug: contactslistsupload-post
      parameters:
      - in: formData
        name: file
        description: CSV file to be uploaded
      - in: formData
        name: name
        description: A name of a contact list
      - in: formData
        name: useCustomFields
        description: A flag to indicate how to define property names for contacts
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Upload