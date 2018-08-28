---
swagger: "2.0"
x-collection-name: Azure Scheduler
x-complete: 0
info:
  title: Azure Scheduler API Jobs List
  version: 1.0.0
  description: Lists all jobs under the specified job collection.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  : get:
      summary: Jobs Get
      description: Gets a job.
      operationId: Jobs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get
      parameters:
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    put:
      summary: Jobs Create Or Update
      description: Provisions a new job or updates an existing job.
      operationId: Jobs_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-put
      parameters:
      - in: body
        name: job
        description: The job definition
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    patch:
      summary: Jobs Patch
      description: Patches an existing job.
      operationId: Jobs_Patch
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-patch
      parameters:
      - in: body
        name: job
        description: The job definition
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    delete:
      summary: Jobs Delete
      description: Deletes a job.
      operationId: Jobs_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete
      parameters:
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}/run
  : post:
      summary: Jobs Run
      description: Runs a job.
      operationId: Jobs_Run
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post
      parameters:
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: path
        name: jobName
        description: The job name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs
  : get:
      summary: Jobs List
      description: Lists all jobs under the specified job collection.
      operationId: Jobs_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the job state
      - in: query
        name: $skip
        description: The (0-based) index of the job history list from which to begin
          requesting entries
      - in: query
        name: $top
        description: The number of jobs to request, in the of range of [1
      - in: path
        name: jobCollectionName
        description: The job collection name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Jobs
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