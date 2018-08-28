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
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Scheduler API Jobs Get
  x-api-slug: azure-scheduler-api
  description: Gets a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-get-openapi.md
- name: Azure Scheduler API Jobs Create Or Update
  x-api-slug: azure-scheduler-api
  description: Provisions a new job or updates an existing job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-put-openapi.md
- name: Azure Scheduler API Jobs Patch
  x-api-slug: azure-scheduler-api
  description: Patches an existing job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-patch-openapi.md
- name: Azure Scheduler API Jobs Delete
  x-api-slug: azure-scheduler-api
  description: Deletes a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobname-delete-openapi.md
- name: Azure Scheduler API Jobs Run
  x-api-slug: azure-scheduler-api
  description: Runs a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}/run
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamerun-post-openapi.md
- name: Azure Scheduler API Jobs List
  x-api-slug: azure-scheduler-api
  description: Lists all jobs under the specified job collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobs-get-openapi.md
- name: Azure Scheduler API Jobs List Job History
  x-api-slug: azure-scheduler-api
  description: Lists job history.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Scheduler/jobCollections/{jobCollectionName}/jobs/{jobName}/history
  tags: Jobs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamehistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-schedulerjobcollectionsjobcollectionnamejobsjobnamehistory-get-openapi.md
- name: Azure Scheduler API
  x-api-slug: azure-scheduler-api
  description: Azure Scheduler lets you create jobs in the cloud that invoke services
    inside and outside of Azure&mdash;such as calling HTTP/S endpoints or posting
    messages to Azure Storage queues, or Azure Service Bus queues or topics. Run jobs
    right away, on a recurring schedule, or at some point in the future.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: ://management.azure.com//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/openapi.md
x-common:
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