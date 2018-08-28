swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/integrations/{integrationID}/jobs/{integrationJobID}/logs:
    get:
      summary: Get Logs for a Job
      description: Get logs for a job.
      operationId: V2IntegrationsJobsLogsByIntegrationIDAndIntegrationJobIDGet
      x-api-path-slug: v2integrationsintegrationidjobsintegrationjobidlogs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      - in: path
        name: integrationJobID
      responses:
        200:
          description: Successful response
      tags:
      - Logsa
      - Job