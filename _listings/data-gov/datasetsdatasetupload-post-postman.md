{
  "info": {
    "name": "Data.gov API Add Datasets Dataset Upload",
    "_postman_id": "33c998c8-4d5c-4973-87cd-055fdfadefa5",
    "description": "Upload a new dataset resource",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "e64cca39-f3f8-4725-b85f-fd18539173eb",
          "name": "postDatasetsDatasetUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/upload/"
              ],
              "variable": [
                {
                  "id": "dataset",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Upload a new dataset resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a13e682a-4e84-4d1b-9d25-bad45d191e1f"
            }
          ]
        }
      ]
    }
  ]
}