---
name: Azure Scheduler
description: Azure Scheduler lets you create jobs in the cloud that invoke services
  inside and outside of Azuremdash;such as calling HTTP/S endpoints or posting messages
  to Azure Storage queues, or Azure Service Bus queues or topics. Run jobs right away,
  on a recurring schedule, or at some point in the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Scheduler
- Orchestration
- Microsoft
- Jobs
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure Scheduler API
  description: Azure Scheduler lets you create jobs in the cloud that invoke services
    inside and outside of Azuremdash;such as calling HTTP/S endpoints or posting messages
    to Azure Storage queues, or Azure Service Bus queues or topics
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-scheduler-jobcollections-jobcollectionname-jobs-jobname-history-get.md
- name: Azure Scheduler API Jobs Run
  description: Runs a job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-scheduler-create.png
  humanURL: https://azure.microsoft.com/en-us/services/scheduler/
  baseURL: http:://management.azure.com//
  tags: Jobs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-scheduler-jobcollections-jobcollectionname-jobs-jobname-run-post.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/azure-scheduler/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-scheduler-jobcollections-jobcollectionname-jobs-jobname-run-post-postman.md
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