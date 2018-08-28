swagger: "2.0"
x-collection-name: Apica
x-complete: 1
info:
  title: Scenarios API
  version: 1.0.0
host: api.pingdom.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
basePath: /
paths:
  '/checks/{checkId}/job ':
    ' get ':
      summary: Get Checks Job
      description: DEPRECATED. Gets the current job status for a check.
      operationId: -checks-checkid-job-
      x-api-path-slug: checkscheckidjob-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Jobs
    ' post ':
      summary: Get Checks Job
      description: Executes a check.
      operationId: -checks-checkid-job-
      x-api-path-slug: checkscheckidjob-post
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Jobs