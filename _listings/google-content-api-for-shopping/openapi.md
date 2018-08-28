swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 1
info:
  title: Content API for Shopping
  description: manages-product-items-inventory-and-merchant-center-accounts-for-google-shopping-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{merchantId}/products:
    post:
      summary: Upload Product
      description: Uploads a product to your Merchant Center account. If an item with
        the same channel, contentLanguage, offerId, and targetCountry already exists,
        this method updates that entry. This method can only be called for non-multi-client
        accounts.
      operationId: content.products.insert
      x-api-path-slug: merchantidproducts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Product