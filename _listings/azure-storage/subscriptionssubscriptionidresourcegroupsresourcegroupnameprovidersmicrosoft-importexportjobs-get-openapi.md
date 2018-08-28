---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Jobs List By Resource Group
  version: 1.0.0
  description: Returns all active and completed import/export jobs in a resource group.
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