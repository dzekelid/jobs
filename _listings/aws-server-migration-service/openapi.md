swagger: "2.0"
x-collection-name: AWS Server Migration Service
x-complete: 1
info:
  title: AWS Server Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetReplicationJobs:
    get:
      summary: Get Replication Jobs
      description: The get-replication-jobs API will return all of your ReplicationJobs
        and their details.
      operationId: getReplicationJobs
      x-api-path-slug: actiongetreplicationjobs-get
      parameters:
      - in: query
        name: maxResults
        description: 'Type: Integer'
        type: string
      - in: query
        name: nextToken
        description: 'Type: String'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Jobs