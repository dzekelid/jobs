---
name: Google Biquery
x-slug: google-biquery
description: BigQuery is Googles fully managed, petabyte scale, low cost enterprise
  data warehouse for analytics. BigQuery is serverless. There is no infrastructure
  to manage and you dont need a database administrator, so you can focus on analyzing
  data to find meaningful insights using familiar SQL. BigQuery is a powerful Big
  Data analytics platform used by all types of organizations, from startups to Fortune
  500 companies.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Jobs
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/apis.md
specificationVersion: "0.14"
apis:
- name: BigQuery - Get Jobs
  x-api-slug: projectsprojectidjobs-get
  description: Lists all jobs that you started in the specified project. Job information
    is available for a six month period after creation. The job list is sorted in
    reverse chronological order, by job creation time. Requires the Can View project
    role, or the Is Owner project role if you set the allUsers property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobs-get-openapi.md
- name: BigQuery - Create Job
  x-api-slug: projectsprojectidjobs-post
  description: Starts a new asynchronous job. Requires the Can View project role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobs-post-openapi.md
- name: BigQuery - Get Job
  x-api-slug: projectsprojectidjobsjobid-get
  description: Returns information about a specific job. Job information is available
    for a six month period after creation. Requires that you're the person who ran
    the job, or have the Is Owner project role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobsjobid-get-openapi.md
- name: BigQuery - Cancel Job
  x-api-slug: projectsprojectidjobsjobidcancel-post
  description: Requests that a job be cancelled. This call will return immediately,
    and the client will need to poll for the job status to see if the cancel completed
    successfully. Cancelled jobs may still incur costs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobsjobidcancel-post-openapi.md
- name: BigQuery - Run Query Job
  x-api-slug: projectsprojectidqueries-post
  description: Runs a BigQuery SQL query synchronously and returns query results if
    the query completes within a specified timeout.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidqueries-post-openapi.md
- name: BigQuery - Get Query Job Results
  x-api-slug: projectsprojectidqueriesjobid-get
  description: Retrieves the results of a query job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidqueriesjobid-get-openapi.md
- name: BigQuery - Get Jobs
  x-api-slug: projectsprojectidjobs-get
  description: Lists all jobs that you started in the specified project. Job information
    is available for a six month period after creation. The job list is sorted in
    reverse chronological order, by job creation time. Requires the Can View project
    role, or the Is Owner project role if you set the allUsers property.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobs-get-openapi.md
- name: BigQuery - Create Job
  x-api-slug: projectsprojectidjobs-post
  description: Starts a new asynchronous job. Requires the Can View project role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobs-post-openapi.md
- name: BigQuery - Get Job
  x-api-slug: projectsprojectidjobsjobid-get
  description: Returns information about a specific job. Job information is available
    for a six month period after creation. Requires that you're the person who ran
    the job, or have the Is Owner project role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobsjobid-get-openapi.md
- name: BigQuery - Cancel Job
  x-api-slug: projectsprojectidjobsjobidcancel-post
  description: Requests that a job be cancelled. This call will return immediately,
    and the client will need to poll for the job status to see if the cancel completed
    successfully. Cancelled jobs may still incur costs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidjobsjobidcancel-post-openapi.md
- name: BigQuery - Run Query Job
  x-api-slug: projectsprojectidqueries-post
  description: Runs a BigQuery SQL query synchronously and returns query results if
    the query completes within a specified timeout.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidqueries-post-openapi.md
- name: BigQuery - Get Query Job Results
  x-api-slug: projectsprojectidqueriesjobid-get
  description: Retrieves the results of a query job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/BigQuery_500px.png
  humanURL: https://cloud.google.com/bigquery/
  baseURL: ://www.googleapis.com//bigquery/v2
  tags: Data, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Databases, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/jobs/master/_listings/google-biquery/projectsprojectidqueriesjobid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.beacons.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.biquery.stack.network
- type: x-code
  url: https://cloud.google.com/bigquery/docs/reference/libraries
- type: x-documentation
  url: https://cloud.google.com/bigquery/docs/
- type: x-getting-started
  url: https://cloud.google.com/bigquery/docs/quickstarts
- type: x-how-to-guides
  url: https://cloud.google.com/bigquery/docs/how-to
- type: x-partners
  url: https://cloud.google.com/bigquery/partners/
- type: x-pricing
  url: https://cloud.google.com/bigquery/pricing
- type: x-quotas
  url: https://cloud.google.com/bigquery/quota-policy
- type: x-service-level-agreement
  url: https://cloud.google.com/bigquery/sla
- type: x-support
  url: https://cloud.google.com/bigquery/support
- type: x-tutorials
  url: https://cloud.google.com/bigquery/docs/tutorials
- type: x-website
  url: https://cloud.google.com/bigquery/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---