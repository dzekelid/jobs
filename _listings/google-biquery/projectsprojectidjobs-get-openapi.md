---
swagger: "2.0"
x-collection-name: Google Biquery
x-complete: 0
info:
  title: Google BigQuery API Get Jobs
  description: Lists all jobs that you started in the specified project. Job information
    is available for a six month period after creation. The job list is sorted in
    reverse chronological order, by job creation time. Requires the Can View project
    role, or the Is Owner project role if you set the allUsers property.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /bigquery/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectId}/jobs:
    get:
      summary: Get Jobs
      description: Lists all jobs that you started in the specified project. Job information
        is available for a six month period after creation. The job list is sorted
        in reverse chronological order, by job creation time. Requires the Can View
        project role, or the Is Owner project role if you set the allUsers property.
      operationId: bigquery.jobs.list
      x-api-path-slug: projectsprojectidjobs-get
      parameters:
      - in: query
        name: allUsers
        description: Whether to display jobs owned by all users in the project
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Page token, returned by a previous call, to request the next
          page of results
      - in: path
        name: projectId
        description: Project ID of the jobs to list
      - in: query
        name: projection
        description: Restrict information returned to a set of selected fields
      - in: query
        name: stateFilter
        description: Filter for job state
      responses:
        200:
          description: OK
      tags:
      - Job
    post:
      summary: Create Job
      description: Starts a new asynchronous job. Requires the Can View project role.
      operationId: bigquery.jobs.insert
      x-api-path-slug: projectsprojectidjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: Project ID of the project that will be billed for the job
      responses:
        200:
          description: OK
      tags:
      - Job
  /projects/{projectId}/jobs/{jobId}:
    get:
      summary: Get Job
      description: Returns information about a specific job. Job information is available
        for a six month period after creation. Requires that you're the person who
        ran the job, or have the Is Owner project role.
      operationId: bigquery.jobs.get
      x-api-path-slug: projectsprojectidjobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: '[Required] Job ID of the requested job'
      - in: path
        name: projectId
        description: '[Required] Project ID of the requested job'
      responses:
        200:
          description: OK
      tags:
      - Job
  /projects/{projectId}/jobs/{jobId}/cancel:
    post:
      summary: Cancel Job
      description: Requests that a job be cancelled. This call will return immediately,
        and the client will need to poll for the job status to see if the cancel completed
        successfully. Cancelled jobs may still incur costs.
      operationId: bigquery.jobs.cancel
      x-api-path-slug: projectsprojectidjobsjobidcancel-post
      parameters:
      - in: path
        name: jobId
        description: '[Required] Job ID of the job to cancel'
      - in: path
        name: projectId
        description: '[Required] Project ID of the job to cancel'
      responses:
        200:
          description: OK
      tags:
      - Job
  /projects/{projectId}/queries:
    post:
      summary: Run Query Job
      description: Runs a BigQuery SQL query synchronously and returns query results
        if the query completes within a specified timeout.
      operationId: bigquery.jobs.query
      x-api-path-slug: projectsprojectidqueries-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: Project ID of the project billed for the query
      responses:
        200:
          description: OK
      tags:
      - Job
  /projects/{projectId}/queries/{jobId}:
    get:
      summary: Get Query Job Results
      description: Retrieves the results of a query job.
      operationId: bigquery.jobs.getQueryResults
      x-api-path-slug: projectsprojectidqueriesjobid-get
      parameters:
      - in: path
        name: jobId
        description: '[Required] Job ID of the query job'
      - in: query
        name: maxResults
        description: Maximum number of results to read
      - in: query
        name: pageToken
        description: Page token, returned by a previous call, to request the next
          page of results
      - in: path
        name: projectId
        description: '[Required] Project ID of the query job'
      - in: query
        name: startIndex
        description: Zero-based index of the starting row
      - in: query
        name: timeoutMs
        description: How long to wait for the query to complete, in milliseconds,
          before returning
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