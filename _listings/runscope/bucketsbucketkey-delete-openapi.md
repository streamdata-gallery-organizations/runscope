---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 0
info:
  title: Runscope Delete Buckets Bucketkey
  description: Delete a single bucket resource.
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: Account Resource
      operationId: account.get
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /buckets:
    get:
      summary: Get Buckets
      description: Returns a list of buckets.
      operationId: buckets.get
      x-api-path-slug: buckets-get
      responses:
        200:
          description: OK
      tags:
      - Buckets
    post:
      summary: Add Buckets
      description: Create a new bucket
      operationId: buckets.post
      x-api-path-slug: buckets-post
      parameters:
      - in: body
        name: NewBucket
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
  /buckets/{bucketKey}:
    delete:
      summary: Delete Buckets Bucketkey
      description: Delete a single bucket resource.
      operationId: buckets.bucketKey.delete
      x-api-path-slug: bucketsbucketkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Bucketkey
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