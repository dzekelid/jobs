---
swagger: "2.0"
x-collection-name: Azure Scheduler
x-complete: 0
info:
  title: Azure Scheduler API Jobs Delete
  version: 1.0.0
  description: Deletes a job.
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