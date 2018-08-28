---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Uploads
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Upload a file
  x-api-slug: files-post
  description: |-
    Uploads a file that can later be attached to a post.

    This request can either be a multipart/form-data request with a channel_id, files and optional
    client_ids defined in the FormData, or it can be a request with the channel_id and filename
    defined as query parameters with the contents of a single file in the body of the request.

    Only multipart/form-data requests are supported by server versions up to and including 4.7.
    Server versions 4.8 and higher support both types of requests.

    ##### Permissions
    Must have `upload_file` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/files-post-openapi.md
- name: Mattermost API Reference - Upload license file
  x-api-slug: license-post
  description: |-
    Upload a license to enable enterprise features.

    __Minimum server version__: 4.0

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/license-post-openapi.md
- name: Mattermost API Reference - Upload IDP certificate
  x-api-slug: samlcertificateidp-post
  description: |-
    Upload the IDP certificate to be used with your SAML configuration. This will also set the filename for the IdpCertificateFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificateidp-post-openapi.md
- name: Mattermost API Reference - Upload public certificate
  x-api-slug: samlcertificatepublic-post
  description: |-
    Upload the public certificate to be used for encryption with your SAML configuration. This will also set the filename for the PublicCertificateFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificatepublic-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificatepublic-post-openapi.md
- name: Mattermost API Reference - Upload private key
  x-api-slug: samlcertificateprivate-post
  description: |-
    Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificateprivate-post-openapi.md
- name: Mattermost API Reference - Upload brand image
  x-api-slug: brandimage-post
  description: |-
    Uploads a brand image.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/brandimage-post-openapi.md
- name: Mattermost API Reference - Upload plugin
  x-api-slug: plugins-post
  description: |-
    Upload a plugin compressed in a .tar.gz file. Plugins and plugin uploads must be enabled in the server's config settings.

    ##### Permissions
    Must have `manage_system` permission.

    __Minimum server version__: 4.4
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/plugins-post-openapi.md
- name: Mattermost API Reference - Upload plugin
  x-api-slug: plugins-post
  description: |-
    Upload a plugin compressed in a .tar.gz file. Plugins and plugin uploads must be enabled in the server's config settings.

    ##### Permissions
    Must have `manage_system` permission.

    __Minimum server version__: 4.4
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/plugins-post-openapi.md
- name: Mattermost API Reference - Upload brand image
  x-api-slug: brandimage-post
  description: |-
    Uploads a brand image.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/brandimage-post-openapi.md
- name: Mattermost API Reference - Upload private key
  x-api-slug: samlcertificateprivate-post
  description: |-
    Upload the private key to be used for encryption with your SAML configuration. This will also set the filename for the PrivateKeyFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificateprivate-post-openapi.md
- name: Mattermost API Reference - Upload public certificate
  x-api-slug: samlcertificatepublic-post
  description: |-
    Upload the public certificate to be used for encryption with your SAML configuration. This will also set the filename for the PublicCertificateFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificatepublic-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificatepublic-post-openapi.md
- name: Mattermost API Reference - Upload IDP certificate
  x-api-slug: samlcertificateidp-post
  description: |-
    Upload the IDP certificate to be used with your SAML configuration. This will also set the filename for the IdpCertificateFile setting in your `config.json`.
    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/samlcertificateidp-post-openapi.md
- name: Mattermost API Reference - Upload license file
  x-api-slug: license-post
  description: |-
    Upload a license to enable enterprise features.

    __Minimum server version__: 4.0

    ##### Permissions
    Must have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/license-post-openapi.md
- name: Mattermost API Reference - Upload a file
  x-api-slug: files-post
  description: |-
    Uploads a file that can later be attached to a post.

    This request can either be a multipart/form-data request with a channel_id, files and optional
    client_ids defined in the FormData, or it can be a request with the channel_id and filename
    defined as query parameters with the contents of a single file in the body of the request.

    Only multipart/form-data requests are supported by server versions up to and including 4.7.
    Server versions 4.8 and higher support both types of requests.

    ##### Permissions
    Must have `upload_file` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/mattermost/files-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---