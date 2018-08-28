---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Upload Server Certificate
  version: 1.0.0
  description: Uploads a server certificate entity for the AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UploadServerCertificate:
    get:
      summary: Upload Server Certificate
      description: Uploads a server certificate entity for the AWS account.
      operationId: uploadServerCertificate
      x-api-path-slug: actionuploadservercertificate-get
      parameters:
      - in: query
        name: CertificateBody
        description: The contents of the public key certificate in PEM-encoded format
        type: string
      - in: query
        name: CertificateChain
        description: The contents of the certificate chain
        type: string
      - in: query
        name: Path
        description: The path for the server certificate
        type: string
      - in: query
        name: PrivateKey
        description: The contents of the private key in PEM-encoded format
        type: string
      - in: query
        name: ServerCertificateName
        description: The name for the server certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=UploadSigningCertificate:
    get:
      summary: Upload Signing Certificate
      description: Uploads an X.
      operationId: uploadSigningCertificate
      x-api-path-slug: actionuploadsigningcertificate-get
      parameters:
      - in: query
        name: CertificateBody
        description: The contents of the signing certificate
        type: string
      - in: query
        name: UserName
        description: The name of the user the signing certificate is for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=UploadSSHPublicKey:
    get:
      summary: Upload S S H Public Key
      description: Uploads an SSH public key and associates it with the specified
        IAM user.
      operationId: uploadSSHPublicKey
      x-api-path-slug: actionuploadsshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyBody
        description: The SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to associate the SSH public key with
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
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