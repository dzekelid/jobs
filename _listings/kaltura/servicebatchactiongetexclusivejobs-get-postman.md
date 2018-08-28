{
  "info": {
    "name": "Kaltura VPaaS Get Service Batch Action Getexclusivejobs",
    "_postman_id": "2f39260e-2c77-464e-855d-823a0dbc4d82",
    "description": "batch getExclusiveJobsAction action allows to get a BatchJob",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "6846220d-d977-40d2-8649-2d7591526169",
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
              "id": "f61988d5-8844-45af-ab93-1d37acc699a9"
            }
          ]
        },
        {
          "id": "b8561c2a-aaff-466d-8329-459057a88961",
          "name": "batch.addMediaInfo",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/addMediaInfo?mediaInfo[audioBitRateMode]=%7B%7D&mediaInfo[audioBitRate]=%7B%7D&mediaInfo[audioChannels]=%7B%7D&mediaInfo[audioCodecId]=%7B%7D&mediaInfo[audioDuration]=%7B%7D&mediaInfo[audioFormat]=%7B%7D&mediaInfo[audioResolution]=%7B%7D&mediaInfo[audioSamplingRate]=%7B%7D&mediaInfo[complexityValue]=%7B%7D&mediaInfo[containerBitRate]=%7B%7D&mediaInfo[containerDuration]=%7B%7D&mediaInfo[containerFormat]=%7B%7D&mediaInfo[containerId]=%7B%7D&mediaInfo[containerProfile]=%7B%7D&mediaInfo[contentStreams]=%7B%7D&mediaInfo[fileSize]=%7B%7D&mediaInfo[flavorAssetId]=%7B%7D&mediaInfo[isFastStart]=%7B%7D&mediaInfo[maxGOP]=%7B%7D&mediaInfo[multiStreamInfo]=%7B%7D&mediaInfo[multiStream]=%7B%7D&mediaInfo[rawData]=%7B%7D&mediaInfo[scanType]=%7B%7D&mediaInfo[videoBitRateMode]=%7B%7D&mediaInfo[videoBitRate]=%7B%7D&mediaInfo[videoCodecId]=%7B%7D&mediaInfo[videoDar]=%7B%7D&mediaInfo[videoDuration]=%7B%7D&mediaInfo[videoFormat]=%7B%7D&mediaInfo[videoFrameRate]=%7B%7D&mediaInfo[videoHeight]=%7B%7D&mediaInfo[videoRotation]=%7B%7D&mediaInfo[videoWidth]=%7B%7D&mediaInfo[writingLib]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch addMediaInfoAction action saves a media info object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "154231d1-93aa-4f0f-be5a-10a267fe1b4c"
            }
          ]
        },
        {
          "id": "9f31ea00-89e6-46cf-8ba6-98c2f951d7e9",
          "name": "batch.checkEntryIsDone",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/checkEntryIsDone?batchJobId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch checkEntryIsDone Check weather a specified entry is done converting and changes it to ready."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e68ea19-f418-4bd1-bf01-b8fca25f2036"
            }
          ]
        },
        {
          "id": "7460e7b8-bcb2-4ea5-8748-c93ce5fe19af",
          "name": "batch.checkFileExists",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/checkFileExists?localPath=%7B%7D&No Name=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch checkFileExists action check if the file exists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87dd7cd5-8b15-4f28-a637-30dfc480cf86"
            }
          ]
        },
        {
          "id": "f12b66b2-fbfe-4df5-a51e-52fab2963fd1",
          "name": "batch.cleanExclusiveJobs",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/cleanExclusiveJobs?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch cleanExclusiveJobs action mark as fatal error all expired jobs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed4f7e08-46ca-472a-9f54-ae5c52672d64"
            }
          ]
        },
        {
          "id": "44bfcf8a-9708-4441-a1ca-8ef24bfce22f",
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
              "id": "d94c6262-d922-45c9-837f-4e7db1a44db7"
            }
          ]
        },
        {
          "id": "54e218cd-3eab-4f19-bbd2-ba88fc6563fa",
          "name": "batch.freeExclusiveJob",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/freeExclusiveJob?id=%7B%7D&jobType=%7B%7D&lockKey[batchIndex]=%7B%7D&lockKey[schedulerId]=%7B%7D&lockKey[workerId]=%7B%7D&No Name=%7B%7D&resetExecutionAttempts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch freeExclusiveJobAction action allows to get a generic BatchJob"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c68eec5-5208-48a1-8214-3054e1537078"
            }
          ]
        },
        {
          "id": "93a71018-cd4a-4c49-ae6a-1106dd96c02b",
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
              "id": "e40a333f-c2f5-496e-9352-aa4ae5737dc8"
            }
          ]
        },
        {
          "id": "a2304b52-35c4-4bd2-923d-cb1c28456483",
          "name": "batch.getExclusiveAlmostDone",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/getExclusiveAlmostDone?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[batchVersionEqual]=%7B%7D&filter[batchVersionGreaterThanOrEqual]=%7B%7D&filter[batchVersionLessThanOrEqual]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[errNumberEqual]=%7B%7D&filter[errNumberIn]=%7B%7D&filter[errNumberNotIn]=%7B%7D&filter[errTypeEqual]=%7B%7D&filter[errTypeIn]=%7B%7D&filter[errTypeNotIn]=%7B%7D&filter[estimatedEffortGreaterThan]=%7B%7D&filter[estimatedEffortLessThan]=%7B%7D&filter[executionAttemptsGreaterThanOrEqual]=%7B%7D&filter[executionAttemptsLessThanOrEqual]=%7B%7D&filter[finishTimeGreaterThanOrEqual]=%7B%7D&filter[finishTimeLessThanOrEqual]=%7B%7D&filter[idEqual]=%7B%7D&filter[idGreaterThanOrEqual]=%7B%7D&filter[jobSubTypeEqual]=%7B%7D&filter[jobSubTypeIn]=%7B%7D&filter[jobSubTypeNotIn]=%7B%7D&filter[jobTypeAndSubTypeIn]=%7B%7D&filter[jobTypeEqual]=%7B%7D&filter[jobTypeIn]=%7B%7D&filter[jobTypeNotIn]=%7B%7D&filter[lockVersionGreaterThanOrEqual]=%7B%7D&filter[lockVersionLessThanOrEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[partnerIdNotIn]=%7B%7D&filter[priorityEqual]=%7B%7D&filter[priorityGreaterThanOrEqual]=%7B%7D&filter[priorityIn]=%7B%7D&filter[priorityLessThanOrEqual]=%7B%7D&filter[priorityNotIn]=%7B%7D&filter[queueTimeGreaterThanOrEqual]=%7B%7D&filter[queueTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[urgencyGreaterThanOrEqual]=%7B%7D&filter[urgencyLessThanOrEqual]=%7B%7D&jobType=%7B%7D&lockKey[batchIndex]=%7B%7D&lockKey[schedulerId]=%7B%7D&lockKey[workerId]=%7B%7D&maxExecutionTime=%7B%7D&No Name=%7B%7D&numberOfJobs=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch getExclusiveAlmostDone action allows to get a BatchJob that wait for remote closure"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b01188d3-f0c2-423d-a5f3-a99a7bceb29a"
            }
          ]
        },
        {
          "id": "9e8e500b-1b27-4fb8-8436-a4d5380712da",
          "name": "batch.getExclusiveJobs",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/batch/action/getExclusiveJobs?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[batchVersionEqual]=%7B%7D&filter[batchVersionGreaterThanOrEqual]=%7B%7D&filter[batchVersionLessThanOrEqual]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[entryIdEqual]=%7B%7D&filter[errNumberEqual]=%7B%7D&filter[errNumberIn]=%7B%7D&filter[errNumberNotIn]=%7B%7D&filter[errTypeEqual]=%7B%7D&filter[errTypeIn]=%7B%7D&filter[errTypeNotIn]=%7B%7D&filter[estimatedEffortGreaterThan]=%7B%7D&filter[estimatedEffortLessThan]=%7B%7D&filter[executionAttemptsGreaterThanOrEqual]=%7B%7D&filter[executionAttemptsLessThanOrEqual]=%7B%7D&filter[finishTimeGreaterThanOrEqual]=%7B%7D&filter[finishTimeLessThanOrEqual]=%7B%7D&filter[idEqual]=%7B%7D&filter[idGreaterThanOrEqual]=%7B%7D&filter[jobSubTypeEqual]=%7B%7D&filter[jobSubTypeIn]=%7B%7D&filter[jobSubTypeNotIn]=%7B%7D&filter[jobTypeAndSubTypeIn]=%7B%7D&filter[jobTypeEqual]=%7B%7D&filter[jobTypeIn]=%7B%7D&filter[jobTypeNotIn]=%7B%7D&filter[lockVersionGreaterThanOrEqual]=%7B%7D&filter[lockVersionLessThanOrEqual]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[partnerIdNotIn]=%7B%7D&filter[priorityEqual]=%7B%7D&filter[priorityGreaterThanOrEqual]=%7B%7D&filter[priorityIn]=%7B%7D&filter[priorityLessThanOrEqual]=%7B%7D&filter[priorityNotIn]=%7B%7D&filter[queueTimeGreaterThanOrEqual]=%7B%7D&filter[queueTimeLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[urgencyGreaterThanOrEqual]=%7B%7D&filter[urgencyLessThanOrEqual]=%7B%7D&jobType=%7B%7D&lockKey[batchIndex]=%7B%7D&lockKey[schedulerId]=%7B%7D&lockKey[workerId]=%7B%7D&maxExecutionTime=%7B%7D&maxJobToPullForCache=%7B%7D&No Name=%7B%7D&numberOfJobs=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "batch getExclusiveJobsAction action allows to get a BatchJob"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68279734-b917-4ade-b161-931bed1e35d0"
            }
          ]
        }
      ]
    }
  ]
}