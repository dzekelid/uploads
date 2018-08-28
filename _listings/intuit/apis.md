---
name: Intuit
x-slug: intuit
description: See how the power of Intuit Giants can work for you by joining the over
  46 million people already using TurboTax, QuickBooks and Mint to power their financial
  prosperity.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
x-kinRank: "8"
x-alexaRank: "263"
tags: Uploads
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/apis.md
specificationVersion: "0.14"
apis:
- name: QuickBooks Online V3 API - Post Upload
  x-api-slug: upload-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
  humanURL: https://intuit.com
  baseURL: https://DefaultParameterValue//v3/company/DefaultParameterValue
  tags: Finance, Accounting, Orange Report Financial, Finance, Accounting, Stack Network,
    Stack, Financial Services, SaaS, Technology, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/upload-post-openapi.md
- name: QuickBooks Online V3 API - Post Upload
  x-api-slug: upload-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
  humanURL: https://intuit.com
  baseURL: https://DefaultParameterValue//v3/company/DefaultParameterValue
  tags: Finance, Accounting, Orange Report Financial, Finance, Accounting, Stack Network,
    Stack, Financial Services, SaaS, Technology, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/upload-post-openapi.md
- name: QuickBooks Online V3 API - Post Upload
  x-api-slug: upload-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
  humanURL: https://intuit.com
  baseURL: https://DefaultParameterValue//v3/company/DefaultParameterValue
  tags: Finance, Accounting, Orange Report Financial, Finance, Accounting, Stack Network,
    Stack, Financial Services, SaaS, Technology, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/upload-post-openapi.md
- name: QuickBooks Online V3 API - Post Upload
  x-api-slug: upload-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
  humanURL: https://intuit.com
  baseURL: https://DefaultParameterValue//v3/company/DefaultParameterValue
  tags: Finance, Accounting, Orange Report Financial, Finance, Accounting, Stack Network,
    Stack, Financial Services, SaaS, Technology, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/upload-post-openapi.md
- name: QuickBooks Online V3 API - Post Upload
  x-api-slug: upload-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/9544-intuit.jpg
  humanURL: https://intuit.com
  baseURL: https://DefaultParameterValue//v3/company/DefaultParameterValue
  tags: Finance, Accounting, Orange Report Financial, Finance, Accounting, Stack Network,
    Stack, Financial Services, SaaS, Technology, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/uploads/master/_listings/intuit/upload-post-openapi.md
x-common:
- type: x-postman-collection
  url: https://www.getpostman.com/collections/554420530884cde6b794
- type: x-api-gallery
  url: http://intrinio.api.gallery.streamdata.io
- type: x-api-stack
  url: http://intuit.stack.network
- type: x-base
  url: https://appcenter.intuit.com/api/
- type: x-blog
  url: https://developer.intuit.com/blog
- type: x-blog-rss
  url: https://developer.intuit.com/blog/feed
- type: x-crunchbase
  url: https://crunchbase.com/organization/intuit
- type: x-developer
  url: https://developer.intuit.com/
- type: x-email
  url: copyright@intuit.com
- type: x-email
  url: spoof@intuit.com
- type: x-github
  url: https://github.com/IntuitDeveloperRelations
- type: x-partners
  url: https://developer.intuit.com/partnerprogram
- type: x-road-map
  url: https://developer.intuit.com/blog/2013/12/19/2014-roadmap-and-migration-dates-for-existing-developers
- type: x-twitter
  url: https://twitter.com/Intuit
- type: x-twitter
  url: https://twitter.com/intuitdev
- type: x-website
  url: https://intuit.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---