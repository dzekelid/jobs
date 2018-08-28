swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListUserImportJobs:
    get:
      summary: List User Import Jobs
      description: Lists the user import jobs.
      operationId: listUserImportJobs
      x-api-path-slug: actionlistuserimportjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of import jobs you want the request to return
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to ListUserImportJobs,
          which            can be used to return the next set of import jobs in the
          list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports