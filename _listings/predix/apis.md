---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Jobs
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Analytics Framework - Get all job definition entries.
  x-api-slug: apiv1schedulerjobs-get
  description: Returns all job definition entries as specified by page and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-get-openapi.md
- name: Analytics Framework - Create a scheduler job.
  x-api-slug: apiv1schedulerjobs-post
  description: Creates the scheduler job with a generated id. Set the state value
    to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
    the job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-post-openapi.md
- name: Analytics Framework - Get a scheduler job by id.
  x-api-slug: apiv1schedulerjobsid-get
  description: Returns the scheduler job with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-get-openapi.md
- name: Analytics Framework - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Framework - Delete job definition.
  x-api-slug: apiv1schedulerjobsid-delete
  description: Delete job definition for the given job id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-delete-openapi.md
- name: Analytics Framework - Retrieve job execution history of the given job.
  x-api-slug: apiv1schedulerjobsidhistory-get
  description: Retrieve job execution history
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsidhistory-get-openapi.md
- name: Analytics Framework - Retrieve job execution history of the given job.
  x-api-slug: apiv1schedulerjobsidhistory-get
  description: Retrieve job execution history
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsidhistory-get-openapi.md
- name: Analytics Framework - Delete job definition.
  x-api-slug: apiv1schedulerjobsid-delete
  description: Delete job definition for the given job id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-delete-openapi.md
- name: Analytics Framework - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Framework - Get a scheduler job by id.
  x-api-slug: apiv1schedulerjobsid-get
  description: Returns the scheduler job with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-get-openapi.md
- name: Analytics Framework - Create a scheduler job.
  x-api-slug: apiv1schedulerjobs-post
  description: Creates the scheduler job with a generated id. Set the state value
    to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
    the job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-post-openapi.md
- name: Analytics Framework - Get all job definition entries.
  x-api-slug: apiv1schedulerjobs-get
  description: Returns all job definition entries as specified by page and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-get-openapi.md
- name: Analytics Runtime - Get all job definition entries.
  x-api-slug: apiv1schedulerjobs-get
  description: Returns all job definition entries as specified by page and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-get-openapi.md
- name: Analytics Runtime - Create a scheduler job.
  x-api-slug: apiv1schedulerjobs-post
  description: Creates the scheduler job with a generated id. Set the state value
    to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
    the job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-post-openapi.md
- name: Analytics Runtime - Get a scheduler job by id.
  x-api-slug: apiv1schedulerjobsid-get
  description: Returns the scheduler job with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-get-openapi.md
- name: Analytics Runtime - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Runtime - Delete job definition.
  x-api-slug: apiv1schedulerjobsid-delete
  description: Delete job definition for the given job id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-delete-openapi.md
- name: Analytics Runtime - Retrieve job execution history of the given job.
  x-api-slug: apiv1schedulerjobsidhistory-get
  description: Retrieve job execution history
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsidhistory-get-openapi.md
- name: Analytics Runtime - Retrieve job execution history of the given job.
  x-api-slug: apiv1schedulerjobsidhistory-get
  description: Retrieve job execution history
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsidhistory-get-openapi.md
- name: Analytics Runtime - Delete job definition.
  x-api-slug: apiv1schedulerjobsid-delete
  description: Delete job definition for the given job id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-delete-openapi.md
- name: Analytics Runtime - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Runtime - Get a scheduler job by id.
  x-api-slug: apiv1schedulerjobsid-get
  description: Returns the scheduler job with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobsid-get-openapi.md
- name: Analytics Runtime - Create a scheduler job.
  x-api-slug: apiv1schedulerjobs-post
  description: Creates the scheduler job with a generated id. Set the state value
    to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
    the job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-post-openapi.md
- name: Analytics Runtime - Get all job definition entries.
  x-api-slug: apiv1schedulerjobs-get
  description: Returns all job definition entries as specified by page and sort criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/predix/apiv1schedulerjobs-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---