swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Job:
    get:
      summary: Gets the status for a job given its reference
      description: Gets the status for a job given its reference.
      operationId: Job_GetJobStatusByjobReference
      x-api-path-slug: apijob-get
      parameters:
      - in: query
        name: jobReference
        description: The job reference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Statusa
      - Job
      - Given
      - Its
      - Reference
    post:
      summary: Issues a request that a job be cancelled if possbile
      description: Issues a request that a job be cancelled if possbile.
      operationId: Job_CancelJobBycancellationRequest
      x-api-path-slug: apijob-post
      parameters:
      - in: body
        name: cancellationRequest
        description: The cancellation request
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Request
      - That
      - Job
      - Be
      - Cancelled
      - If
      - Possbile
  /api/admin/system/sendliveportalupdatemessage:
    post:
      summary: "Sends a message to the LivePortalJobHandler that says \r\nthe specified
        property marketing role has changed"
      description: "Sends a message to the liveportaljobhandler that says \r\nthe
        specified property marketing role has changed."
      operationId: System_SendLivePortalUpdateMessageBypropertyMarketingRoleId
      x-api-path-slug: apiadminsystemsendliveportalupdatemessage-post
      parameters:
      - in: query
        name: propertyMarketingRoleId
        description: The property marketing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Message
      - To
      - LivePortalJobHandler
      - That
      - Says
      - The
      - Specified
      - Property
      - Marketing
      - Role
      - Has
      - Changed