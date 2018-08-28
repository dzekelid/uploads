---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Get Uploaded
  description: Return a list of books uploaded by the current user.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /volumes/useruploaded:
    get:
      summary: Get Uploaded
      description: Return a list of books uploaded by the current user.
      operationId: books.volumes.useruploaded.list
      x-api-path-slug: volumesuseruploaded-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: processingState
        description: The processing state of the user uploaded volumes to be returned
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      - in: query
        name: volumeId
        description: The ids of the volumes to be returned
      responses:
        200:
          description: OK
      tags:
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