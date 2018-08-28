---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API Describe Job Flows
  version: 1.0.0
  description: This API is deprecated and will eventually be removed.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddJobFlowSteps:
    get:
      summary: Add Job Flow Steps
      description: AddJobFlowSteps adds new steps to a running job flow.
      operationId: addJobFlowSteps
      x-api-path-slug: actionaddjobflowsteps-get
      parameters:
      - in: query
        name: JobFlowId
        description: A string that uniquely identifies the job flow
        type: string
      - in: query
        name: Steps
        description: A list of StepConfig to be executed by the job flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flow Steps
  /?Action=DescribeJobFlows:
    get:
      summary: Describe Job Flows
      description: This API is deprecated and will eventually be removed.
      operationId: describeJobFlows
      x-api-path-slug: actiondescribejobflows-get
      parameters:
      - in: query
        name: CreatedAfter
        description: Return only job flows created after this date and time
        type: string
      - in: query
        name: CreatedBefore
        description: Return only job flows created before this date and time
        type: string
      - in: query
        name: JobFlowIds
        description: Return only job flows whose job flow ID is contained in this
          list
        type: string
      - in: query
        name: JobFlowStates
        description: Return only job flows whose state is contained in this list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flows
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