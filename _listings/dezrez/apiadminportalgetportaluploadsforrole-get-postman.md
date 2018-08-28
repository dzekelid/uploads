{
  "info": {
    "name": "Dezrez Get all the live portal uploads associated with a property marketing role",
    "_postman_id": "0f3e332c-0c2e-4457-b822-8b377ef82548",
    "description": "Get all the live portal uploads associated with a property marketing role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "d7b61d28-162c-4663-8430-73a449efd918",
          "name": "AccountingSystem_GetOfficeAccounts",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/officeaccounts",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get list of office accounts associated with the accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21319f65-3f5e-4d2c-8740-186a4265e126"
            }
          ]
        }
      ]
    },
    {
      "name": "Returns",
      "item": [
        {
          "id": "6e614c2e-d444-494b-bece-7f1dc2aa9ee6",
          "name": "DocumentGeneration_GetLetterTemplateByletterTemplateId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/lettertemplate/:letterTemplateId"
              ],
              "variable": [
                {
                  "id": "letterTemplateId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of lettertemplates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e4f3cf0-1569-4903-ab43-86d084a0cd9d"
            }
          ]
        },
        {
          "id": "3b81678c-4d58-4c1f-ba92-a3155eda4906",
          "name": "DocumentGeneration_GetPrintableMergeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/mergetemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of lettertemplates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ff7c44d-fb0d-42de-99c7-421ca189bb1a"
            }
          ]
        },
        {
          "id": "8f4ded74-47d2-47ff-8650-b6d8e533d987",
          "name": "DocumentGeneration_GetUnusedMergeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/unusedmergetemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of lettertemplates associated to this agency that are not currently used in any envelope templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fdf8463-fd84-4fb0-845d-912a84cabbb4"
            }
          ]
        },
        {
          "id": "f7b66eef-d761-47d7-943d-03fb80dec7ed",
          "name": "DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/templatesusinganalytics/:analyticsId"
              ],
              "variable": [
                {
                  "id": "analyticsId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of lettertemplates associated to this agency and to a particular google analyitics campaign."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5af8c912-9a10-45a6-bafa-2baa53a3f351"
            }
          ]
        },
        {
          "id": "1972f3a8-e2e1-45bd-bd42-ad9627f25239",
          "name": "DocumentGeneration_GetPrintableInsertableTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/insertabletemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of insertable templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bd515ab-aba3-458f-9173-4b614ffa641d"
            }
          ]
        },
        {
          "id": "bffa0858-a7c5-465b-8a35-f089964ae928",
          "name": "DocumentGeneration_GetPrintableHeaderTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/headertemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of header templates associated to this agency with their associated brand info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0e07df3-a0c2-484d-bd88-68683e5af394"
            }
          ]
        },
        {
          "id": "ef961d2d-ed1b-41b2-9a6b-577d801b2259",
          "name": "DocumentGeneration_GetEnvelopeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of envelope templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "014a1bdf-cc76-400c-9c40-9d2f844847d9"
            }
          ]
        },
        {
          "id": "b57b7f27-4a29-4db0-8ab2-11107a67962c",
          "name": "DocumentGeneration_GetEnvelopeTemplatePacks",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplatepacks",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of envelope template packs associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa96ad2f-ebc5-41fb-9fd7-975d1ad742aa"
            }
          ]
        },
        {
          "id": "455b75ca-54cb-4b35-8742-a0a4da8b5108",
          "name": "DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplatepacktypes?inUseOnly=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of envelope template packs associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12854585-e848-4516-bc59-4a86a1078689"
            }
          ]
        },
        {
          "id": "bbe452a6-dd73-42ab-a72b-e8b2dbb967e3",
          "name": "DocumentGeneration_GetEmailTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/emailtemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of email templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecea1910-1c18-491c-b3e9-7a108209d860"
            }
          ]
        },
        {
          "id": "dd14b341-798e-4ec5-83c0-be60a67bbb19",
          "name": "DocumentGeneration_GetTemplatesBytemplateType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/templates/:templateType"
              ],
              "variable": [
                {
                  "id": "templateType",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of mergable templates for any type associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4563f6a-c53e-4a37-abc9-de047f70eafd"
            }
          ]
        },
        {
          "id": "c2d20708-3737-47b1-9988-773c398575be",
          "name": "DocumentGeneration_GetSmsTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/smstemplates",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sms templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "791383b1-91ac-48a1-b0d3-6694f0a4d11d"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "b553fcd3-dfc1-4c58-930e-a6d6f194039c",
          "name": "Portal_GetLivePortalInformationRecordsForRoleByroleId",
          "request": {
            "url": "http://api.dezrez.com/api/admin/portal/getportaluploadsforrole?roleId=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all the live portal uploads associated with a property marketing role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7378b7be-cd60-4151-8c75-d17776a1e69c"
            }
          ]
        }
      ]
    }
  ]
}