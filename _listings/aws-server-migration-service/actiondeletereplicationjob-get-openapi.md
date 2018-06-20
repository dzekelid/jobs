---
swagger: "2.0"
x-collection-name: AWS Server Migration Service
x-complete: 0
info:
  title: AWS Server Migration Service API Delete Replication Job
  version: 1.0.0
  description: The delete-replication-job API is used to delete a ReplicationJob,
    resulting in no further ReplicationRuns.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateReplicationJob:
    get:
      summary: Create Replication Job
      description: The create-replication-job API is used to create a ReplicationJob
        to replicate a server on AWS.
      operationId: createReplicationJob
      x-api-path-slug: actioncreatereplicationjob-get
      parameters:
      - in: query
        name: description
        description: 'Type: String'
        type: string
      - in: query
        name: frequency
        description: 'Type: Integer'
        type: string
      - in: query
        name: licenseType
        description: 'Type: String'
        type: string
      - in: query
        name: roleName
        description: 'Type: String'
        type: string
      - in: query
        name: seedReplicationTime
        description: 'Type: Timestamp'
        type: string
      - in: query
        name: serverId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Jobs
  /?Action=DeleteReplicationJob:
    get:
      summary: Delete Replication Job
      description: The delete-replication-job API is used to delete a ReplicationJob,
        resulting in no further ReplicationRuns.
      operationId: deleteReplicationJob
      x-api-path-slug: actiondeletereplicationjob-get
      parameters:
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Jobs
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