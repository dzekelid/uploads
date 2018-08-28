{
  "info": {
    "name": "Kaltura VPaaS Get Service Bulkupload Bulk Action List",
    "_postman_id": "a085cffb-4087-4e03-a2a2-85b977ef0bf8",
    "description": "List bulk upload batch jobs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "153266e1-b589-475e-a5ac-c4470a0e5e41",
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
              "id": "32f5dfae-9736-4c39-85b6-ff2f28a6994e"
            }
          ]
        },
        {
          "id": "3e52dde8-9bfd-4bcf-bf64-d0f5ace80aed",
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
              "id": "ee948e52-ba9e-484e-8871-7cd55bafcd6e"
            }
          ]
        },
        {
          "id": "02cb3f6c-eda1-4409-bdb2-ee9876391b5f",
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
              "id": "a6b5a3b5-3c67-4f5d-a02c-c6765888836b"
            }
          ]
        },
        {
          "id": "f6a6dcff-ceb1-462e-bbed-f83291f5551d",
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
              "id": "c53dea21-0387-40b4-9baf-7c7785fe4bd6"
            }
          ]
        },
        {
          "id": "e1ff72ec-1a70-4da2-9d5f-11760fff569f",
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
              "id": "2f588628-e855-4073-bad2-fbd5d53186a5"
            }
          ]
        },
        {
          "id": "fec1d8a7-c6d1-445a-8212-13a66220dfdd",
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
              "id": "ef813b29-73a6-4a29-9c13-dec7accda27e"
            }
          ]
        },
        {
          "id": "215270cf-4f0a-4eb3-9b2c-5d4452539c4b",
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
              "id": "4635a70e-aebf-4c12-83f1-897f74cbe4bf"
            }
          ]
        },
        {
          "id": "e7e2cf47-1353-4a0d-bf2d-0651024c8a79",
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
              "id": "90b21f78-ff9d-4385-b7d4-210ef804e582"
            }
          ]
        },
        {
          "id": "fb060ebe-58ad-4cec-80fa-7cc296c47cb6",
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
              "id": "07fec16a-a283-400c-a039-9d28ff2ecbc7"
            }
          ]
        },
        {
          "id": "184432f6-0c84-4141-9400-09c8535a005e",
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
              "id": "ef2b5147-f8cc-4f04-8819-97eabe65f346"
            }
          ]
        },
        {
          "id": "e6e5d9a4-3ee4-4fc7-9808-66aa5bf97ef5",
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
              "id": "f30f3a02-5324-42d6-8701-2aa33e7c7a91"
            }
          ]
        },
        {
          "id": "2ace61b0-4312-44bc-a540-b418f97635df",
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
              "id": "6f24cbb1-16d4-4777-b4ff-2b6536217a9d"
            }
          ]
        },
        {
          "id": "5a41d9dd-43f2-445e-b276-aa6c19b4aeac",
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
              "id": "006eb62f-9e21-40fd-ae04-43cf2300f40d"
            }
          ]
        },
        {
          "id": "25b5132e-dc29-42b6-87c8-f0458c24c860",
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
              "id": "a4254608-a81f-49c8-a0f9-3629c12b1eb4"
            }
          ]
        },
        {
          "id": "ead483cf-06ec-4642-951c-193f0db1b165",
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
              "id": "a8f6a467-73cb-4cf3-8ead-bb5ec9e1a3e8"
            }
          ]
        }
      ]
    }
  ]
}