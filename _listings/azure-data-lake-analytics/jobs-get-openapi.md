---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Job List
  description: Lists the jobs, if any, associated with the specified Data Lake Analytics
    account. The response includes a link to the next page of results, if any.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Jobs/{jobIdentity}:
    get:
      summary: Job Get
      description: Gets the job information for the specified job ID.
      operationId: Job_Get
      x-api-path-slug: jobsjobidentity-get
      parameters:
      - in: path
        name: jobIdentity
        description: JobInfo ID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
    put:
      summary: Job Create
      description: Submits a job to the specified Data Lake Analytics account.
      operationId: Job_Create
      x-api-path-slug: jobsjobidentity-put
      parameters:
      - in: path
        name: jobIdentity
        description: The job ID (a GUID) for the job being submitted
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters to submit a job
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
  /Jobs:
    get:
      summary: Job List
      description: Lists the jobs, if any, associated with the specified Data Lake
        Analytics account. The response includes a link to the next page of results,
        if any.
      operationId: Job_List
      x-api-path-slug: jobs-get
      parameters:
      - in: query
        name: $count
        description: The Boolean value of true or false to request a count of the
          matching resources included with the resources in the response, e
      - in: query
        name: $filter
        description: OData filter
      - in: query
        name: $orderby
        description: OrderBy clause
      - in: query
        name: $select
        description: OData Select statement
      - in: query
        name: $skip
        description: The number of items to skip over before returning elements
      - in: query
        name: $top
        description: The number of items to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
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