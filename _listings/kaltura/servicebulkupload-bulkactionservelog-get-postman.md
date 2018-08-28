{
  "info": {
    "name": "Kaltura VPaaS Get Service Bulkupload Bulk Action Servelog",
    "_postman_id": "05ead0c8-a515-4283-93dd-d8506d03d66f",
    "description": "serveLog action returns the log file for the bulk-upload job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "667a1eed-14fb-4509-92c2-a8cc1b72ebbf",
          "name": "annotation.addFromBulk",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/addFromBulk?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "fileData",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Allows you to add multiple cue points objects by uploading XML that contains multiple cue point definitions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32320e8e-549f-4098-a458-f67add9c0203"
            }
          ]
        },
        {
          "id": "f6829eb5-1396-43a2-b4d4-dfcd56ed8b95",
          "name": "annotation.serveBulk",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/annotation_annotation/action/serveBulk?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[codeEqual]=%7B%7D&filter[codeIn]=%7B%7D&filter[codeLike]=%7B%7D&filter[codeMultiLikeAnd]=%7B%7D&filter[codeMultiLikeOr]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[cuePointTypeEqual]=%7B%7D&filter[cuePointTypeIn]=%7B%7D&filter[descriptionLike]=%7B%7D&filter[descriptionMultiLikeAnd]=%7B%7D&filter[descriptionMultiLikeOr]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[endTimeGreaterThanOrEqual]=%7B%7D&filter[endTimeLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[entryIdIn]=%7B%7D&filter[eventTypeEqual]=%7B%7D&filter[eventTypeIn]=%7B%7D&filter[forceStopEqual]=%7B%7D&filter[freeText]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[isPublicEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentIdEqual]=%7B%7D&filter[parentIdIn]=%7B%7D&filter[partnerSortValueEqual]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueIn]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[protocolTypeEqual]=%7B%7D&filter[protocolTypeIn]=%7B%7D&filter[questionLike]=%7B%7D&filter[questionMultiLikeAnd]=%7B%7D&filter[questionMultiLikeOr]=%7B%7D&filter[quizUserEntryIdEqual]=%7B%7D&filter[quizUserEntryIdIn]=%7B%7D&filter[startTimeGreaterThanOrEqual]=%7B%7D&filter[startTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[subTypeEqual]=%7B%7D&filter[subTypeIn]=%7B%7D&filter[systemNameEqual]=%7B%7D&filter[systemNameIn]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[textLike]=%7B%7D&filter[textMultiLikeAnd]=%7B%7D&filter[textMultiLikeOr]=%7B%7D&filter[titleLike]=%7B%7D&filter[titleMultiLikeAnd]=%7B%7D&filter[titleMultiLikeOr]=%7B%7D&filter[triggeredAtGreaterThanOrEqual]=%7B%7D&filter[triggeredAtLessThanOrEqual]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdCurrent]=%7B%7D&filter[userIdEqualCurrent]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download multiple cue points objects as XML definitions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a510206-fff4-4590-b7a7-f5f5cf6e51c0"
            }
          ]
        },
        {
          "id": "05855e03-fc93-4f69-aa5a-46696f61d516",
          "name": "batch.addBulkUploadResult",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/addBulkUploadResult?bulkUploadResult[accessControlProfileId]=%7B%7D&bulkUploadResult[action]=%7B%7D&bulkUploadResult[appearInList]=%7B%7D&bulkUploadResult[bulkUploadJobId]=%7B%7D&bulkUploadResult[bulkUploadResultObjectType]=%7B%7D&bulkUploadResult[categoryId]=%7B%7D&bulkUploadResult[categoryReferenceId]=%7B%7D&bulkUploadResult[category]=%7B%7D&bulkUploadResult[city]=%7B%7D&bulkUploadResult[contentType]=%7B%7D&bulkUploadResult[contributionPolicy]=%7B%7D&bulkUploadResult[conversionProfileId]=%7B%7D&bulkUploadResult[country]=%7B%7D&bulkUploadResult[creatorId]=%7B%7D&bulkUploadResult[dateOfBirth]=%7B%7D&bulkUploadResult[defaultPermissionLevel]=%7B%7D&bulkUploadResult[description]=%7B%7D&bulkUploadResult[email]=%7B%7D&bulkUploadResult[entitledUsersEdit]=%7B%7D&bulkUploadResult[entitledUsersPublish]=%7B%7D&bulkUploadResult[entryId]=%7B%7D&bulkUploadResult[entryStatus]=%7B%7D&bulkUploadResult[errorCode]=%7B%7D&bulkUploadResult[errorDescription]=%7B%7D&bulkUploadResult[errorType]=%7B%7D&bulkUploadResult[firstName]=%7B%7D&bulkUploadResult[gender]=%7B%7D&bulkUploadResult[group]=%7B%7D&bulkUploadResult[inheritanceType]=%7B%7D&bulkUploadResult[lastName]=%7B%7D&bulkUploadResult[lineIndex]=%7B%7D&bulkUploadResult[moderation]=%7B%7D&bulkUploadResult[name]=%7B%7D&bulkUploadResult[objectErrorDescription]=%7B%7D&bulkUploadResult[objectId]=%7B%7D&bulkUploadResult[objectStatus]=%7B%7D&bulkUploadResult[objectType]=%7B%7D&bulkUploadResult[ownerId]=%7B%7D&bulkUploadResult[owner]=%7B%7D&bulkUploadResult[parentSystemName]=%7B%7D&bulkUploadResult[parentType]=%7B%7D&bulkUploadResult[partnerData]=%7B%7D&bulkUploadResult[partnerId]=%7B%7D&bulkUploadResult[partnerSortValue]=%7B%7D&bulkUploadResult[permissionLevel]=%7B%7D&bulkUploadResult[pluginsData]=%7B%7D&bulkUploadResult[privacy]=%7B%7D&bulkUploadResult[referenceId]=%7B%7D&bulkUploadResult[relativePath]=%7B%7D&bulkUploadResult[requiredObjectStatus]=%7B%7D&bulkUploadResult[resourceId]=%7B%7D&bulkUploadResult[rowData]=%7B%7D&bulkUploadResult[scheduleEndDate]=%7B%7D&bulkUploadResult[scheduleStartDate]=%7B%7D&bulkUploadResult[screenName]=%7B%7D&bulkUploadResult[sshKeyPassphrase]=%7B%7D&bulkUploadResult[sshPrivateKey]=%7B%7D&bulkUploadResult[sshPublicKey]=%7B%7D&bulkUploadResult[state]=%7B%7D&bulkUploadResult[status]=%7B%7D&bulkUploadResult[systemName]=%7B%7D&bulkUploadResult[tags]=%7B%7D&bulkUploadResult[templateEntryId]=%7B%7D&bulkUploadResult[thumbnailSaved]=%7B%7D&bulkUploadResult[thumbnailUrl]=%7B%7D&bulkUploadResult[title]=%7B%7D&bulkUploadResult[type]=%7B%7D&bulkUploadResult[updateMethod]=%7B%7D&bulkUploadResult[url]=%7B%7D&bulkUploadResult[userId]=%7B%7D&bulkUploadResult[userJoinPolicy]=%7B%7D&bulkUploadResult[zip]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch addBulkUploadResultAction action adds KalturaBulkUploadResult to the DB"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac96f5cd-18a4-4155-826d-ef67225b5a15"
            }
          ]
        },
        {
          "id": "54960e2f-af87-4ceb-9b9c-ad3a584f6772",
          "name": "batch.countBulkUploadEntries",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/countBulkUploadEntries?bulkUploadJobId=%7B%7D&bulkUploadObjectType=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total created entries count and total error entries count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c87461d6-f769-43c5-a39a-81e19b71e3ed"
            }
          ]
        },
        {
          "id": "eefd06ca-9e7e-441f-9319-2e21279807f9",
          "name": "batch.getBulkUploadLastResult",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/getBulkUploadLastResult?bulkUploadJobId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch getBulkUploadLastResultAction action returns the last result of the bulk upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "734d19d9-a193-46ef-8223-cb0090eba990"
            }
          ]
        },
        {
          "id": "ac536309-cc23-4832-9d8c-beb487ff6d0f",
          "name": "batch.updateBulkUploadResults",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/updateBulkUploadResults?bulkUploadJobId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch updateBulkUploadResults action adds KalturaBulkUploadResult to the DB"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1faa04f-6c5d-46da-9760-a792a9df3632"
            }
          ]
        },
        {
          "id": "450412e3-9f0f-485c-8da6-517fc2b55b01",
          "name": "bulkUpload.abort",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/abort?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Aborts the bulk upload and all its child jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9f94af3-578b-45d2-8b57-5b95da62923b"
            }
          ]
        },
        {
          "id": "1730f314-58ee-4081-83cf-155d30df99fc",
          "name": "bulkUpload.add",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/add?bulkUploadType=%7B%7D&conversionProfileId=%7B%7D&fileName=%7B%7D&No Name=%7B%7D&uploadedBy=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "csvFileData",
                  "value": "{}",
                  "disabled": false,
                  "description": "bulk upload file"
                }
              ]
            },
            "description": "Add new bulk upload batch job\n\nConversion profile id can be specified in the API or in the CSV file, the one in the CSV file will be stronger.\n\nIf no conversion profile was specified, partner's default will be used"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f057712f-13f7-4792-a7e9-d92d1a24d3bd"
            }
          ]
        },
        {
          "id": "77ef7921-2197-4103-8637-521ebeebbb69",
          "name": "bulkUpload.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/get?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get bulk upload batch job by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a51902e-5d68-49bd-aa52-10795d63a051"
            }
          ]
        },
        {
          "id": "395dc7c5-8d73-4cbe-8eb6-100eeb35ca33",
          "name": "bulkUpload.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/list?No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List bulk upload batch jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4c66f18-1d37-4a11-b7ed-cd722a1b912b"
            }
          ]
        },
        {
          "id": "6d95bbde-9d20-4a3d-80a7-a39076dc7e1c",
          "name": "bulkUpload.serve",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/serve?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "serve action returan the original file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0bb5c45-6f2e-4b28-b512-e67e1371b1a4"
            }
          ]
        },
        {
          "id": "085f0185-f52e-4e60-840b-8ceae1220498",
          "name": "bulkUpload.serveLog",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload/action/serveLog?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "serveLog action returan the original file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b541c785-8159-4d4c-851a-62e1e76101db"
            }
          ]
        },
        {
          "id": "de521842-bbd7-468c-a6b8-50f731d8da8b",
          "name": "bulk.abort",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload_bulk/action/abort?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Aborts the bulk upload and all its child jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52123930-ba5f-4866-8650-f60aad4d9173"
            }
          ]
        },
        {
          "id": "8b9b2946-2f04-4871-8c96-cee4cf93d929",
          "name": "bulk.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload_bulk/action/get?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get bulk upload batch job by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475fff01-e2f7-4d2a-a682-89f7a13852f7"
            }
          ]
        },
        {
          "id": "424df73a-3553-4795-ad2d-a5b33501ee5f",
          "name": "bulk.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload_bulk/action/list?bulkUploadFilter[advancedSearch][attribute]=%7B%7D&bulkUploadFilter[advancedSearch][categoriesMatchOr]=%7B%7D&bulkUploadFilter[advancedSearch][categoryEntryStatusIn]=%7B%7D&bulkUploadFilter[advancedSearch][categoryIdEqual]=%7B%7D&bulkUploadFilter[advancedSearch][comparison]=%7B%7D&bulkUploadFilter[advancedSearch][contentLike]=%7B%7D&bulkUploadFilter[advancedSearch][contentMultiLikeAnd]=%7B%7D&bulkUploadFilter[advancedSearch][contentMultiLikeOr]=%7B%7D&bulkUploadFilter[advancedSearch][cuePointsFreeText]=%7B%7D&bulkUploadFilter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&bulkUploadFilter[advancedSearch][cuePointTypeIn]=%7B%7D&bulkUploadFilter[advancedSearch][depthGreaterThanEqual]=%7B%7D&bulkUploadFilter[advancedSearch][distributionProfileId]=%7B%7D&bulkUploadFilter[advancedSearch][distributionSunStatus]=%7B%7D&bulkUploadFilter[advancedSearch][entryDistributionFlag]=%7B%7D&bulkUploadFilter[advancedSearch][entryDistributionStatus]=%7B%7D&bulkUploadFilter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&bulkUploadFilter[advancedSearch][extendedStatusEqual]=%7B%7D&bulkUploadFilter[advancedSearch][extendedStatusIn]=%7B%7D&bulkUploadFilter[advancedSearch][field]=%7B%7D&bulkUploadFilter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&bulkUploadFilter[advancedSearch][idEqual]=%7B%7D&bulkUploadFilter[advancedSearch][idIn]=%7B%7D&bulkUploadFilter[advancedSearch][indexIdGreaterThan]=%7B%7D&bulkUploadFilter[advancedSearch][isQuiz]=%7B%7D&bulkUploadFilter[advancedSearch][items]=%7B%7D&bulkUploadFilter[advancedSearch][memberIdEq]=%7B%7D&bulkUploadFilter[advancedSearch][memberIdIn]=%7B%7D&bulkUploadFilter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&bulkUploadFilter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&bulkUploadFilter[advancedSearch][metadataProfileId]=%7B%7D&bulkUploadFilter[advancedSearch][noDistributionProfiles]=%7B%7D&bulkUploadFilter[advancedSearch][not]=%7B%7D&bulkUploadFilter[advancedSearch][objectType]=%7B%7D&bulkUploadFilter[advancedSearch][orderBy]=%7B%7D&bulkUploadFilter[advancedSearch][type]=%7B%7D&bulkUploadFilter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&bulkUploadFilter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&bulkUploadFilter[advancedSearch][userIdEqual]=%7B%7D&bulkUploadFilter[advancedSearch][userIdIn]=%7B%7D&bulkUploadFilter[advancedSearch][value]=%7B%7D&bulkUploadFilter[advancedSearch][watermarkId]=%7B%7D&bulkUploadFilter[bulkUploadObjectTypeEqual]=%7B%7D&bulkUploadFilter[bulkUploadObjectTypeIn]=%7B%7D&bulkUploadFilter[orderBy]=%7B%7D&bulkUploadFilter[statusEqual]=%7B%7D&bulkUploadFilter[statusIn]=%7B%7D&bulkUploadFilter[uploadedOnEqual]=%7B%7D&bulkUploadFilter[uploadedOnGreaterThanOrEqual]=%7B%7D&bulkUploadFilter[uploadedOnLessThanOrEqual]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List bulk upload batch jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "effcdf69-4d20-4f77-98b2-822cf4252d69"
            }
          ]
        },
        {
          "id": "16919051-8e12-4eac-b23b-ff3725743fd2",
          "name": "bulk.serve",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload_bulk/action/serve?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "serve action returns the original file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5af688b7-ae8a-4a3a-b02c-350f1d710bd7"
            }
          ]
        },
        {
          "id": "f35e916d-9e5d-43ad-98e1-6af232b8a163",
          "name": "bulk.serveLog",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/bulkupload_bulk/action/serveLog?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "serveLog action returns the log file for the bulk-upload job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4964ec4-78e1-42ea-a87d-791fb42e4624"
            }
          ]
        }
      ]
    }
  ]
}