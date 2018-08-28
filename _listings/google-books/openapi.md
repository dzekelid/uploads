swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
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