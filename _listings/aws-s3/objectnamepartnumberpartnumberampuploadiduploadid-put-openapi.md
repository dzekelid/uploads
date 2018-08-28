---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 Upload Part
  version: 1.0.0
  description: This operation uploads a part in a multipart upload
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?uploads:
    get:
      summary: List Multipart Uploads
      description: This operation lists in-progress multipart uploads
      operationId: list-multipart-uploads
      x-api-path-slug: uploads-get
      parameters:
      - in: query
        name: delimiter
        description: Character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Together with upload-id-marker, this parameter specifies the
          multiparttttttttttupload after which listing should begin
      - in: query
        name: max-uploads
        description: Sets the maximum number of multipart uploads, from 1 to 1,000,
          to return in thetttttttttresponse body
      - in: query
        name: prefix
        description: Lists in-progress uploads only for those keys that begin with
          the specified prefix
      - in: query
        name: upload-id-&#8203;marker
        description: Together with key-marker, specifies the multipart upload after
          whichtttttttttlisting should begin
      responses:
        200:
          description: OK
      tags:
      - List
      - Multipart
      - Uploads
  /ObjectName?partNumber=PartNumber&amp;uploadId=UploadId:
    put:
      summary: Upload Part
      description: This operation uploads a part in a multipart upload
      operationId: upload-part
      x-api-path-slug: objectnamepartnumberpartnumberampuploadiduploadid-put
      parameters:
      - in: query
        name: AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo;
          API Reference &raquo; Operations on Objects &raquo; Upload Part - Copy
      - in: header
        name: Content-Length
        description: The size of the part, in bytes
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the part data
      - in: header
        name: Expect
        description: When your application uses 100-continue, it does not send the
          request body until ittttttttttreceives an acknowledgment
      - in: header
        name: x-amz-copy-source
        description: The name of the source bucket and the source object key name
          separated by a                  slash (/)
      - in: header
        name: x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies algorithm to use when decrypting the source object
      - in: header
        name: x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer provided base-64 encoded encryption key
          for Amazon                      S3 to use to decrypt the source object
      - in: header
        name: x-amz-copy-source-&#8203;server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption
          key                      according to RFC 1321
      - in: header
        name: x-amz-copy-source-if-match
        description: Perform a copy if the source object entity tag (ETag) matches
          the specified                  value
      - in: header
        name: x-amz-copy-source-if-modified-since
        description: Perform a copy if the source object is modified after the time
          specified                  using this header
      - in: header
        name: x-amz-copy-source-if-none-match
        description: Perform a copy if the source object entity tag (ETag) is different
          than the                  value specified using this header
      - in: header
        name: x-amz-copy-source-if-unmodified-since
        description: Perform a copy if the source object is not modified after the
          time                  specified using this header
      - in: header
        name: x-amz-copy-source-range
        description: The range of bytes to copy from the source object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when encrypting the object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          for Amazon S3 to use intttttttttttttencrypting data
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption
          key according to RFC 1321
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Part
  /ObjectName?uploadId=UploadId:
    delete:
      summary: Abort Multipart Upload
      description: This operation aborts a multipart upload
      operationId: abort-multipart-upload
      x-api-path-slug: objectnameuploadiduploadid-delete
      responses:
        200:
          description: OK
      tags:
      - Abort
      - Multipart
      - Upload
    post:
      summary: Complete Multipart Upload
      description: This operation completes a multipart upload by assembling previously
        uploaded parts
      operationId: complete-multipart-upload
      x-api-path-slug: objectnameuploadiduploadid-post
      responses:
        200:
          description: OK
      tags:
      - Complete
      - Multipart
      - Upload
  /ObjectName?uploads:
    post:
      summary: Initiate Multipart Upload
      description: This operation initiates a multipart upload and returns an upload
        ID
      operationId: initiate-multipart-upload
      x-api-path-slug: objectnameuploads-post
      parameters:
      - in: header
        name: Cache-Control
        description: Can be used to specify caching behavior along the request/reply
          chain
      - in: header
        name: Content-&#8203;Disposition
        description: Specifies presentational information for the object
      - in: header
        name: Content-Encoding
        description: Specifies what content encodings have been applied to the object
          and thus                  what decoding mechanisms must be applied to obtain
          the media-type referenced by                  the Content-Type header field
      - in: header
        name: Content-Type
        description: A standard MIME type describing the format of the object data
      - in: header
        name: Expires
        description: The date and time at which the object is no longer cacheable
      - in: header
        name: x-amz-acl
        description: The canned ACL to apply to the object
      - in: header
        name: x-amz-grant-full-control
        description: Allows grantee the READ, READ_ACP, and WRITE_ACP permissions
          on the                        object
      - in: header
        name: x-amz-grant-read
        description: Allows grantee to read the object data and its metadata
      - in: header
        name: x-amz-grant-read-acp
        description: Allows grantee to read the object ACL
      - in: header
        name: x-amz-grant-write
        description: Not applicable
      - in: header
        name: x-amz-grant-write-acp
        description: Allows grantee to write the ACL for the applicable object
      - in: header
        name: x-amz-meta-
        description: Headers starting with this prefix are user-defined metadata
      - in: header
        name: x-amz-server-side&#8203;-encryption
        description: Specifies a server-side encryption algorithm to use when Amazon
          S3 creates                        an object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when encrypting the                          object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          for                          Amazon S3 to use in encrypting data
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption                          key
          according to RFC                            1321
      - in: header
        name: x-amz-server-side-encryption-aws-kms-key-id
        description: If the x-amz-server-side-encryption is present and has                        the
          value of aws:kms, this header specifies the ID of the AWS                        Key
          Management Service (KMS) master encryption key that was used for the                        object
      - in: header
        name: x-amz-server-side-encryption-context
        description: If x-amz-server-side-encryption is present, and if its                        value
          is aws:kms, this header specifies the encryption context                        for
          the object
      - in: header
        name: x-amz-storage-&#8203;class
        description: The type of storage to use for the object that is created after
          successful                  multipart upload
      - in: header
        name: x-amz-website&#8203;-redirect-location
        description: If the bucket is configured as a website, redirect requests for
          this object                  to another object in the same bucket or to
          an external URL
      responses:
        200:
          description: OK
      tags:
      - Initiate
      - Multipart
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