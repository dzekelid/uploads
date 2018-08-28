swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files:
    post:
      summary: Upload a file
      description: |-
        Uploads a file that can later be attached to a post.

        This request can either be a multipart/form-data request with a channel_id, files and optional
        client_ids defined in the FormData, or it can be a request with the channel_id and filename
        defined as query parameters with the contents of a single file in the body of the request.

        Only multipart/form-data requests are supported by server versions up to and including 4.7.
        Server versions 4.8 and higher support both types of requests.

        ##### Permissions
        Must have `upload_file` permission.
      operationId: uploads-a-file-that-can-later-be-attached-to-a-postthis-request-can-either-be-a-multipartformdata-re
      x-api-path-slug: files-post
      parameters:
      - in: formData
        name: channel_id
        description: The ID of the channel that this file will be uploaded to
      - in: query
        name: channel_id
        description: The ID of the channel that this file will be uploaded to
      - in: formData
        name: client_ids
        description: A unique identifier for the file that will be returned in the
          response
      - in: query
        name: filename
        description: The ID of the channel that this file will be uploaded to
      - in: formData
        name: files
        description: A file to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
  /license:
    post:
      summary: Upload license file
      description: |-
        Upload a license to enable enterprise features.

        __Minimum server version__: 4.0

        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-a-license-to-enable-enterprise-features-minimum-server-version--40-permissionsmust-have-manag
      x-api-path-slug: license-post
      parameters:
      - in: formData
        name: license
        description: The license to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - License
      - File
  /saml/certificate/idp:
    post:
      summary: Upload IDP certificate
      description: |-
        Upload the IDP certificate to be used with your SAML configuration. This will also set the filename for the IdpCertificateFile setting in your `config.json`.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-the-idp-certificate-to-be-used-with-your-saml-configuration-this-will-also-set-the-filename-f
      x-api-path-slug: samlcertificateidp-post
      parameters:
      - in: formData
        name: certificate
        description: The IDP certificate file
      responses:
        200:
          description: OK
      tags:
      - Upload
      - IDP
      - Certificate
  /saml/certificate/public:
    post:
      summary: Upload public certificate
      description: |-
        Upload the public certificate to be used for encryption with your SAML configuration. This will also set the filename for the PublicCertificateFile setting in your `config.json`.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-the-public-certificate-to-be-used-for-encryption-with-your-saml-configuration-this-will-also-
      x-api-path-slug: samlcertificatepublic-post
      parameters:
      - in: formData
        name: certificate
        description: The public certificate file
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Public
      - Certificate
  /saml/certificate/private:
    post:
      summary: Upload private key
      description: |-
        Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-the-private-key-to-be-used-for-encryption-with-your-saml-configuration-this-will-also-set-the
      x-api-path-slug: samlcertificateprivate-post
      parameters:
      - in: formData
        name: certificate
        description: The private key file
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Private
      - Key
  /brand/image:
    post:
      summary: Upload brand image
      description: |-
        Uploads a brand image.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: uploads-a-brand-image-permissionsmust-have-manage-system-permission
      x-api-path-slug: brandimage-post
      parameters:
      - in: formData
        name: image
        description: The image to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Brand
      - Image
  /plugins:
    post:
      summary: Upload plugin
      description: |-
        Upload a plugin compressed in a .tar.gz file. Plugins and plugin uploads must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: upload-a-plugin-compressed-in-a-targz-file-plugins-and-plugin-uploads-must-be-enabled-in-the-servers
      x-api-path-slug: plugins-post
      parameters:
      - in: formData
        name: plugin
        description: The plugin image to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Plugin