---
name: Azure Scheduler
x-slug: azure-scheduler
description: Azure Scheduler lets you create jobs in the cloud that invoke services
  inside and outside of Azure&mdash;such as calling HTTP/S endpoints or posting messages
  to Azure Storage queues, or Azure Service Bus queues or topics. Run jobs right away,
  on a recurring schedule, or at some point in the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Jobs
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/apis.md
specificationVersion: "0.14"
apis:
- name: SchedulerManagementClient - Jobs Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get
  description: Gets a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get-openapi.md
- name: SchedulerManagementClient - Jobs Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-put
  description: Provisions a new job or updates an existing job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-put-openapi.md
- name: SchedulerManagementClient - Jobs Patch
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-patch
  description: Patches an existing job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-patch-openapi.md
- name: SchedulerManagementClient - Jobs Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete
  description: Deletes a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete-openapi.md
- name: SchedulerManagementClient - Jobs Run
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post
  description: Runs a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post-openapi.md
- name: SchedulerManagementClient - Jobs List
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get
  description: Lists all jobs under the specified job collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get-openapi.md
- name: SchedulerManagementClient - Jobs List Job History
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamehistory-get
  description: Lists job history.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Microsoft, Orchestration, Jobs, Stack Network, API Service Provider, API Provider,
    Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamehistory-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.resource.manager.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.scheduler.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/scheduler/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/scheduler/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/scheduler/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/scheduler/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---