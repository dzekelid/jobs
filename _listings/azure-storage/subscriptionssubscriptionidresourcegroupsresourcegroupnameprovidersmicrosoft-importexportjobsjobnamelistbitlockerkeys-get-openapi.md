---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Jobs List Bit Locker Keys
  version: 1.0.0
  description: Lists the BitLocker keys for all drives in the specified import/export
    job.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.ImportExport/jobs:
    get:
      summary: Jobs List
      description: Gets all the active and completed import/export jobs in a subscription.
      operationId: Jobs_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-importexportjobs-get
      parameters:
      - in: query
        name: $filter
        description: Can be used to restrict the results to certain conditions
      - in: query
        name: $top
        description: An integer value that specifies how many jobs at most should
          be returned
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ImportExport/jobs:
    get:
      summary: Jobs List By Resource Group
      description: Returns all active and completed import/export jobs in a resource
        group.
      operationId: Jobs_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobs-get
      parameters:
      - in: query
        name: $filter
        description: Can be used to restrict the results to certain conditions
      - in: query
        name: $top
        description: An integer value that specifies how many jobs at most should
          be returned
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs Resource Group
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ImportExport/jobs/{jobName}:
    get:
      summary: Jobs Get
      description: Gets information about an existing import/export job.
      operationId: Jobs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobsjobname-get
      parameters:
      - in: path
        name: jobName
        description: The name of the import/export job
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    patch:
      summary: Jobs Update
      description: Updates specific properties of the import/export job. You can call
        this operation to notify the Import/Export service that the hard drives comprising
        the import or export job have been shipped to the Microsoft data center. It
        can also be used to cancel an existing job.
      operationId: Jobs_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobsjobname-patch
      parameters:
      - in: path
        name: jobName
        description: The name of the import/export job
      - in: body
        name: jobProperties
        description: Import/export job properties that need to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    put:
      summary: Jobs Create Or Update
      description: Creates a new import/export job or updates an existing import/export
        job in the specified subscription.
      operationId: Jobs_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobsjobname-put
      parameters:
      - in: path
        name: jobName
        description: The name of the import/export job
      - in: body
        name: jobProperties
        description: Properties of the import/export job that need to be specified
          during creation
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
    delete:
      summary: Jobs Delete
      description: Deletes an existing import/export job. Only import/export jobs
        in the Creating or Completed states can be deleted.
      operationId: Jobs_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobsjobname-delete
      parameters:
      - in: path
        name: jobName
        description: The name of the import/export job
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ImportExport/moveResources:
    post:
      summary: Jobs Move
      description: Moves the specified import/export jobs from the resource group
        to a target resource group. The target resource group may be in a different
        subscription.
      operationId: Jobs_Move
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportmoveresources-post
      parameters:
      - in: body
        name: MoveJobsParameters
        description: Parameters to be provided to move a job from one resource group
          to another
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Jobs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ImportExport/jobs/{jobName}/listBitLockerKeys
  : get:
      summary: Jobs List Bit Locker Keys
      description: Lists the BitLocker keys for all drives in the specified import/export
        job.
      operationId: Jobs_ListBitLockerKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-importexportjobsjobnamelistbitlockerkeys-get
      parameters:
      - in: path
        name: jobName
        description: The name of the import/export job
      - in: query
        name: No Name
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