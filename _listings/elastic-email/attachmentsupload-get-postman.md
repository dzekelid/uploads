{
  "info": {
    "name": "Elastic Email SMTP API Upload Attachment",
    "_postman_id": "4777a13d-87a9-4c45-920e-715b198f8d7f",
    "description": "The upload attachment command is used to upload an attachment for sending.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "3813be20-0c61-464c-86a2-089f4f45da07",
          "name": "getAttachmentsUpload",
          "request": {
            "url": "http://api.elasticemail.com/attachments/upload/?api_key=%7B%7D&file=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The upload attachment command is used to upload an attachment for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54c205c3-29b5-4e19-8f83-b1bdf93add13"
            }
          ]
        }
      ]
    }
  ]
}