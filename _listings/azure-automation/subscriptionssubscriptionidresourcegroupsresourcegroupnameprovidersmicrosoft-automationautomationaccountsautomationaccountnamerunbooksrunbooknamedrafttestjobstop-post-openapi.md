---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Test Jobs Stop
  version: 1.0.0
  description: Stop the test job.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob
  : put:
      summary: Test Jobs Create
      description: Create a test job of the runbook.
      operationId: TestJobs_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjob-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create test job operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: runbookName
        description: The parameters supplied to the create test job operation
      responses:
        200:
          description: OK
      tags:
      - Test
      - Jobs
      - Create
    get:
      summary: Test Jobs Get
      description: Retrieve the test job for the specified runbook.
      operationId: TestJobs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjob-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: runbookName
        description: The runbook name
      responses:
        200:
          description: OK
      tags:
      - Test
      - Jobs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob/resume
  : post:
      summary: Test Jobs Resume
      description: Resume the test job.
      operationId: TestJobs_Resume
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjobresume-post
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: runbookName
        description: The runbook name
      responses:
        200:
          description: OK
      tags:
      - Test
      - Jobs
      - Resume
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob/stop
  : post:
      summary: Test Jobs Stop
      description: Stop the test job.
      operationId: TestJobs_Stop
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjobstop-post
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: runbookName
        description: The runbook name
      responses:
        200:
          description: OK
      tags:
      - Test
      - Jobs
      - Stop
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