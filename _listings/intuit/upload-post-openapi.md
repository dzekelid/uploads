---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Post Upload
  description: "Uploading and linking new attachments\n\nhttps://developer.intuit.com/docs/0100_quickbooks_online/0200_dev_guides/accounting/attachments#Uploading_and_linking_new_attachments\n\nIf
    the attachment is not in the Attachment list already, it's possible to upload
    it and link it to the object in one multipart operation.\n\nOperation:      POST
    https://quickbooks.api.intuit.com/v3/company/companyID/upload\nContent type: multipart/form-data\n\nRequest
    body\n\nThe following sample code shows the multipart request body for uploading
    a file and its supporting Attachable metatdata object, with the result of it being
    both added to the Attachment list and added to the object.\n\nThe Attachable object
    accompanying this request supplies metadata and object information to which the
    attachment is linked. \nEach part of the multipart request is separated by a boundary.
    \ In the sample below, the string  --YOjcLaTlykb6OxfYJx4O07j1MweeMFem is used.
    \ You can use any random and unique string.\nThe file to be uploaded and its Attachable
    object are paired together via the name parameter in the part header for each
    one.\nThe name parameter for the file part is of the form file_content_nn, where
    nn is a unique index number among the set of files being uploaded.\nThe name parameter
    for the Attachable object is of the form file_metadata_nn, where nn corresponds
    to the file index number used with the content .\nThe file or files are stored
    in the Attachment list with the name specified by the filename parameter.\nIf
    the data supplied with the Attachable object cannot be validated, an error is
    returned and the file is not uploaded."
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /upload:
    post:
      summary: Post Upload
      description: "Uploading and linking new attachments\n\nhttps://developer.intuit.com/docs/0100_quickbooks_online/0200_dev_guides/accounting/attachments#Uploading_and_linking_new_attachments\n\nIf
        the attachment is not in the Attachment list already, it's possible to upload
        it and link it to the object in one multipart operation.\n\nOperation:      POST
        https://quickbooks.api.intuit.com/v3/company/companyID/upload\nContent type:
        multipart/form-data\n\nRequest body\n\nThe following sample code shows the
        multipart request body for uploading a file and its supporting Attachable
        metatdata object, with the result of it being both added to the Attachment
        list and added to the object.\n\nThe Attachable object accompanying this request
        supplies metadata and object information to which the attachment is linked.
        \nEach part of the multipart request is separated by a boundary.  In the sample
        below, the string  --YOjcLaTlykb6OxfYJx4O07j1MweeMFem is used.  You can use
        any random and unique string.\nThe file to be uploaded and its Attachable
        object are paired together via the name parameter in the part header for each
        one.\nThe name parameter for the file part is of the form file_content_nn,
        where nn is a unique index number among the set of files being uploaded.\nThe
        name parameter for the Attachable object is of the form file_metadata_nn,
        where nn corresponds to the file index number used with the content .\nThe
        file or files are stored in the Attachment list with the name specified by
        the filename parameter.\nIf the data supplied with the Attachable object cannot
        be validated, an error is returned and the file is not uploaded."
      operationId: postUpload
      x-api-path-slug: upload-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Upload
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