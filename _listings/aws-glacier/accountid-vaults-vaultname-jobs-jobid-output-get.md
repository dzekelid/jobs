---
swagger: "2.0"
info:
  title: Amazon Glacier API Get  Job  Output
  version: 1.0.0
  description: "DescriptionThis operation downloads the output of the job you initiated
    using Initiate Job (POST jobs). Depending\n\t\t\ton the job type you specified
    when you initiated the job, the output will be either the\n\t\t\tcontent of an
    archive or a vault inventory. You can download all the job output or download
    a portion of the output by specifying\n\t\t\ta byte range. For both archive and
    inventory retrieval jobs, you should verify the downloaded \n\t\t\tsize against
    the size returned in the headers from the \n\t\t\tGet Job Output response.For
    archive retrieval jobs, you should also verify that the size is what you expected.
    If\n\t\t\tyou download a portion of the output, the expected size is based on
    the range of bytes\n\t\t\tyou specified. For example, if you specify a range of
    bytes=0-1048575, you should\n\t\t\tverify your download size is 1,048,576 bytes.
    If you download an entire archive, the\n\t\t\texpected size is the size of the
    archive when you uploaded it to Amazon Glacier.\n\t\t\tThe expected size is also
    returned in the headers from the \n\t\t\tGet Job Output response.In the case of
    an archive retrieval job, depending on the byte range you\n\t\t\tspecify, Amazon
    Glacier returns the checksum for the portion of the data. To ensure the portion
    you downloaded \n\t\t\tis the correct data, compute the checksum on the client,
    verify that the values match, \n\t\t\tand verify that the size is what you expected.A
    job ID does not expire for at least 24 hours after Amazon Glacier completes the
    job. That\n\t\t\tis, you can download the job output within the 24-hour period
    after Amazon Glacier\n\t\t\tcompletes the job.Requests"
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{AccountId}/vaults/{VaultName}/jobs/{JobID}/output:
    get:
      summary: Get  Job  Output
      description: DescriptionThis operation downloads the output of the job you initiated
        using Initiate Job (POST jobs)
      operationId: get Job Output (GET output)
      parameters:
      - type: string
      - in: query
        name: ArchiveDescription
        description: The description of an archive
        type: string
      - in: query
        name: ArchiveId
        description: The ID of an archive
        type: string
      - in: query
        name: ArchiveList
        description: An array of archive metadata
        type: string
      - in: query
        name: CreationDate
        description: The UTC date and time the archive was created
        type: string
      - in: query
        name: InventoryDate
        description: "The UTC date and time of the last inventory for the vault that
          was completed after\t\t\t\t\t\t\tchanges to the vault"
        type: string
      - in: query
        name: SHA256TreeHash
        description: The tree hash of the archive
        type: string
      - in: query
        name: Size
        description: The size in bytes of the archive
        type: string
      - in: query
        name: VaultARN
        description: "The Amazon Resource Name (ARN) resource from which the archive\t\t\t\t\t\t\t\tretrieval
          was requested"
        type: string
      responses:
        200:
          description: OK
      tags:
      - jobs
definitions: []
x-collection-name: AWS Glacier
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