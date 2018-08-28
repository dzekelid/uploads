swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 1
info:
  title: Google Analytics
  description: views-and-manages-your-google-analytics-data-
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads:
    get:
      summary: List Uploads
      description: List uploads to which the user has access.
      operationId: analytics.management.uploads.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploads-get
      parameters:
      - in: path
        name: accountId
        description: Account Id for the uploads to retrieve
      - in: path
        name: customDataSourceId
        description: Custom data source Id for uploads to retrieve
      - in: query
        name: max-results
        description: The maximum number of uploads to include in this response
      - in: query
        name: start-index
        description: A 1-based index of the first upload to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for the uploads to retrieve
      responses:
        200:
          description: OK
      tags:
      - Upload
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDataSources/{customDataSourceId}/uploads/{uploadId}:
    get:
      summary: Get UPloads
      description: List uploads to which the user has access.
      operationId: analytics.management.uploads.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdatasourcescustomdatasourceiduploadsuploadid-get
      parameters:
      - in: path
        name: accountId
        description: Account Id for the upload to retrieve
      - in: path
        name: customDataSourceId
        description: Custom data source Id for upload to retrieve
      - in: path
        name: uploadId
        description: Upload Id to retrieve
      - in: path
        name: webPropertyId
        description: Web property Id for the upload to retrieve
      responses:
        200:
          description: OK
      tags:
      - Upload