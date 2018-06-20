---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Batch Action Suspendjobs
  description: batch suspendJobs action suspends jobs from running.
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/batch/action/cleanExclusiveJobs:
    get:
      summary: Get Service Batch Action Cleanexclusivejobs
      description: batch cleanExclusiveJobs action mark as fatal error all expired
        jobs
      operationId: batch.cleanExclusiveJobs
      x-api-path-slug: servicebatchactioncleanexclusivejobs-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - CleanExclusiveJobs
  /service/batch/action/getExclusiveJobs:
    get:
      summary: Get Service Batch Action Getexclusivejobs
      description: batch getExclusiveJobsAction action allows to get a BatchJob
      operationId: batch.getExclusiveJobs
      x-api-path-slug: servicebatchactiongetexclusivejobs-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[batchVersionEqual]
      - in: query
        name: filter[batchVersionGreaterThanOrEqual]
      - in: query
        name: filter[batchVersionLessThanOrEqual]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[errNumberEqual]
      - in: query
        name: filter[errNumberIn]
      - in: query
        name: filter[errNumberNotIn]
      - in: query
        name: filter[errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: filter[errTypeIn]
      - in: query
        name: filter[errTypeNotIn]
      - in: query
        name: filter[estimatedEffortGreaterThan]
      - in: query
        name: filter[estimatedEffortLessThan]
      - in: query
        name: filter[executionAttemptsGreaterThanOrEqual]
      - in: query
        name: filter[executionAttemptsLessThanOrEqual]
      - in: query
        name: filter[finishTimeGreaterThanOrEqual]
      - in: query
        name: filter[finishTimeLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idGreaterThanOrEqual]
      - in: query
        name: filter[jobSubTypeEqual]
      - in: query
        name: filter[jobSubTypeIn]
      - in: query
        name: filter[jobSubTypeNotIn]
      - in: query
        name: filter[jobTypeAndSubTypeIn]
      - in: query
        name: filter[jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: filter[jobTypeIn]
      - in: query
        name: filter[jobTypeNotIn]
      - in: query
        name: filter[lockVersionGreaterThanOrEqual]
      - in: query
        name: filter[lockVersionLessThanOrEqual]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[partnerIdNotIn]
      - in: query
        name: filter[priorityEqual]
      - in: query
        name: filter[priorityGreaterThanOrEqual]
      - in: query
        name: filter[priorityIn]
      - in: query
        name: filter[priorityLessThanOrEqual]
      - in: query
        name: filter[priorityNotIn]
      - in: query
        name: filter[queueTimeGreaterThanOrEqual]
      - in: query
        name: filter[queueTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[urgencyGreaterThanOrEqual]
      - in: query
        name: filter[urgencyLessThanOrEqual]
      - in: query
        name: jobType
        description: 'Enum Type: `KalturaBatchJobType`The type of the job - could
          be a custom extended type'
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: maxExecutionTime
        description: The maximum time in seconds the job reguarly take
      - in: query
        name: maxJobToPullForCache
        description: The number of job to pull to cache
      - in: query
        name: No Name
      - in: query
        name: numberOfJobs
        description: The maximum number of jobs to return
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetExclusiveJobs
  /service/batch/action/getExclusiveNotificationJobs:
    get:
      summary: Get Service Batch Action Getexclusivenotificationjobs
      description: batch getExclusiveNotificationJob action allows to get a BatchJob
        of type NOTIFICATION
      operationId: batch.getExclusiveNotificationJobs
      x-api-path-slug: servicebatchactiongetexclusivenotificationjobs-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[batchVersionEqual]
      - in: query
        name: filter[batchVersionGreaterThanOrEqual]
      - in: query
        name: filter[batchVersionLessThanOrEqual]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[errNumberEqual]
      - in: query
        name: filter[errNumberIn]
      - in: query
        name: filter[errNumberNotIn]
      - in: query
        name: filter[errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: filter[errTypeIn]
      - in: query
        name: filter[errTypeNotIn]
      - in: query
        name: filter[estimatedEffortGreaterThan]
      - in: query
        name: filter[estimatedEffortLessThan]
      - in: query
        name: filter[executionAttemptsGreaterThanOrEqual]
      - in: query
        name: filter[executionAttemptsLessThanOrEqual]
      - in: query
        name: filter[finishTimeGreaterThanOrEqual]
      - in: query
        name: filter[finishTimeLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idGreaterThanOrEqual]
      - in: query
        name: filter[jobSubTypeEqual]
      - in: query
        name: filter[jobSubTypeIn]
      - in: query
        name: filter[jobSubTypeNotIn]
      - in: query
        name: filter[jobTypeAndSubTypeIn]
      - in: query
        name: filter[jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: filter[jobTypeIn]
      - in: query
        name: filter[jobTypeNotIn]
      - in: query
        name: filter[lockVersionGreaterThanOrEqual]
      - in: query
        name: filter[lockVersionLessThanOrEqual]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[partnerIdNotIn]
      - in: query
        name: filter[priorityEqual]
      - in: query
        name: filter[priorityGreaterThanOrEqual]
      - in: query
        name: filter[priorityIn]
      - in: query
        name: filter[priorityLessThanOrEqual]
      - in: query
        name: filter[priorityNotIn]
      - in: query
        name: filter[queueTimeGreaterThanOrEqual]
      - in: query
        name: filter[queueTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[urgencyGreaterThanOrEqual]
      - in: query
        name: filter[urgencyLessThanOrEqual]
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: maxExecutionTime
        description: The maximum time in seconds the job reguarly take
      - in: query
        name: No Name
      - in: query
        name: numberOfJobs
        description: The maximum number of jobs to return
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetExclusiveNotificationJobs
  /service/batch/action/suspendJobs:
    get:
      summary: Get Service Batch Action Suspendjobs
      description: batch suspendJobs action suspends jobs from running.
      operationId: batch.suspendJobs
      x-api-path-slug: servicebatchactionsuspendjobs-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - SuspendJobs
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---