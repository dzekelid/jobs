swagger: "2.0"
x-collection-name: Google Cloud Machine Learning Engine
x-complete: 1
info:
  title: Google Cloud Machine Learning Engine
  description: an-api-to-enable-creating-and-using-machine-learning-models-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: ml.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{parent}/jobs:
    get:
      summary: List Jobs
      description: Lists the jobs in the project.
      operationId: ml.projects.jobs.list
      x-api-path-slug: v1parentjobs-get
      parameters:
      - in: query
        name: filter
        description: Optional
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Job
    post:
      summary: Create Job
      description: Creates a training or a batch prediction job.
      operationId: ml.projects.jobs.create
      x-api-path-slug: v1parentjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Job