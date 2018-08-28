{
  "info": {
    "name": "Kaltura VPaaS Get Service Bulkupload Action List",
    "_postman_id": "b3227756-7c80-42ce-a8d7-c89f2e74445a",
    "description": "List bulk upload batch jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "b7d972a1-adec-4b6b-9796-e08ca9e09952",
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
              "id": "0c684d06-cc8a-4b26-8d90-01558353acae"
            }
          ]
        },
        {
          "id": "7c0a4540-7130-46e7-8240-c6b8ce6b52bb",
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
              "id": "91fa2710-b3c4-4e9e-ab3a-b0d997dd3dda"
            }
          ]
        },
        {
          "id": "7635de2d-f563-4b5d-8190-7eb1f375f752",
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
              "id": "77d329bb-ae76-4752-8b6b-c44d1ac53e5f"
            }
          ]
        },
        {
          "id": "c75b7783-5c14-41be-9868-5a5c9145f849",
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
              "id": "52f827bd-0444-4208-89b2-fc02a716f9cd"
            }
          ]
        },
        {
          "id": "c4b04d21-6839-4972-be72-7ac77d5a5f7b",
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
              "id": "8786a563-c43c-46bd-aee9-06917511f1af"
            }
          ]
        },
        {
          "id": "389ab8ce-f0b3-4f8e-9b0c-ca76d1503b0e",
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
              "id": "feb3a4a7-d261-4be1-b084-563271622c4e"
            }
          ]
        },
        {
          "id": "c17493e5-122f-47cb-be3b-e7f822e3b3a7",
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
              "id": "ff552712-4cde-40ff-871f-28a497add50e"
            }
          ]
        },
        {
          "id": "e74b1353-2173-4b89-99b0-c8c64e15594b",
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
              "id": "88dd03d0-1228-45c4-83c4-2cb815bec2c8"
            }
          ]
        },
        {
          "id": "a7a889dc-21d5-4724-9d8b-f3ad7dfe2907",
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
              "id": "aa441e98-d0eb-4b65-ae88-29608c1bf3e5"
            }
          ]
        },
        {
          "id": "fde4947f-84e5-462d-bb97-a04a4e88e477",
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
              "id": "750fbf12-c421-45e8-899c-99854dce574b"
            }
          ]
        }
      ]
    }
  ]
}