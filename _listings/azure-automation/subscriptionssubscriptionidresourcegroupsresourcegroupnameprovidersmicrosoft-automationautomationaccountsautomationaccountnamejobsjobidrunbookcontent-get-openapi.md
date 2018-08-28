---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Job Get Runbook Content
  version: 1.0.0
  description: Retrieve the runbook content of the job identified by job id.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob/suspend
  : post:
      summary: Test Jobs Suspend
      description: Suspend the test job.
      operationId: TestJobs_Suspend
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjobsuspend-post
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
      - Suspend
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/compilationjobs/{compilationJobId}
  : put:
      summary: Dsc Compilation Job Create
      description: Creates the Dsc compilation job of the configuration.
      operationId: DscCompilationJob_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamecompilationjobscompilationjobid-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: compilationJobId
        description: The the DSC configuration Id
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create compilation job operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Compilation
      - Job
      - Create
    get:
      summary: Dsc Compilation Job Get
      description: Retrieve the Dsc configuration compilation job identified by job
        id.
      operationId: DscCompilationJob_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamecompilationjobscompilationjobid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: compilationJobId
        description: The Dsc configuration compilation job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Compilation
      - Job
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/compilationjobs
  : get:
      summary: Dsc Compilation Job List By Automation Account
      description: Retrieve a list of dsc compilation jobs.
      operationId: DscCompilationJob_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamecompilationjobs-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Compilation
      - Job
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/compilationjobs/{jobId}/streams/{jobStreamId}
  : get:
      summary: Dsc Compilation Job Get Stream
      description: Retrieve the job stream identified by job stream id.
      operationId: DscCompilationJob_GetStream
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamecompilationjobsjobidstreamsjobstreamid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: path
        name: jobStreamId
        description: The job stream id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Compilation
      - Job
      - ""
      - Stream
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/output
  : get:
      summary: Job Get Output
      description: Retrieve the job output identified by job id.
      operationId: Job_GetOutput
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidoutput-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - ""
      - Output
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/runbookContent
  : get:
      summary: Job Get Runbook Content
      description: Retrieve the runbook content of the job identified by job id.
      operationId: Job_GetRunbookContent
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidrunbookcontent-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - ""
      - Runbook
      - Content
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/suspend
  : post:
      summary: Job Suspend
      description: Suspend the job identified by jobId.
      operationId: Job_Suspend
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidsuspend-post
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Suspend
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/stop
  : post:
      summary: Job Stop
      description: Stop the job identified by jobId.
      operationId: Job_Stop
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidstop-post
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Stop
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}
  : get:
      summary: Job Get
      description: Retrieve the job identified by job id.
      operationId: Job_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
    put:
      summary: Job Create
      description: Create a job of the runbook.
      operationId: Job_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobid-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create job operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
      - Create
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs
  : get:
      summary: Job List By Automation Account
      description: Retrieve a list of jobs.
      operationId: Job_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobs-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/resume
  : post:
      summary: Job Resume
      description: Resume the job identified by jobId.
      operationId: Job_Resume
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidresume-post
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Resume
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/streams/{jobStreamId}
  : get:
      summary: Job Stream Get
      description: Retrieve the job stream identified by job stream id.
      operationId: JobStream_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidstreamsjobstreamid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job id
      - in: path
        name: jobStreamId
        description: The job stream id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Stream
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobs/{jobId}/streams
  : get:
      summary: Job Stream List By Job
      description: Retrieve a list of jobs streams identified by job id.
      operationId: JobStream_ListByJob
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobsjobidstreams-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobId
        description: The job Id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Stream
      - ListJob
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobSchedules/{jobScheduleId}
  : delete:
      summary: Job Schedule Delete
      description: Delete the job schedule identified by job schedule name.
      operationId: JobSchedule_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
    get:
      summary: Job Schedule Get
      description: Retrieve the job schedule identified by job schedule name.
      operationId: JobSchedule_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
    put:
      summary: Job Schedule Create
      description: Create a job schedule.
      operationId: JobSchedule_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedulesjobscheduleid-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobScheduleId
        description: The job schedule name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters supplied to the create job schedule operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
      - Create
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/jobSchedules
  : get:
      summary: Job Schedule List By Automation Account
      description: Retrieve a list of job schedules.
      operationId: JobSchedule_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamejobschedules-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Job
      - Schedule
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob/streams/{jobStreamId}
  : get:
      summary: Test Job Streams Get
      description: Retrieve a test job streams identified by runbook name and stream
        id.
      operationId: TestJobStreams_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjobstreamsjobstreamid-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: jobStreamId
        description: The job stream id
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
      - Job
      - Streams
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/runbooks/{runbookName}/draft/testJob/streams
  : get:
      summary: Test Job Streams List By Test Job
      description: Retrieve a list of test job streams identified by runbook name.
      operationId: TestJobStreams_ListByTestJob
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamerunbooksrunbooknamedrafttestjobstreams-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
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
      - Job
      - Streams
      - ListTest
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