---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 0
info:
  title: Runscope Add Buckets Messages
  description: Create a message
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
    get:
      summary: Get Buckets Bucketkey
      description: Returns a single bucket resource.
      operationId: buckets.bucketKey.get
      x-api-path-slug: bucketsbucketkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Bucketkey
  /buckets/{bucketKey}/environments:
    get:
      summary: Get Buckets Environments
      description: Returns list of shared environments for a specified bucket.
      operationId: buckets.bucketKey.environments.get
      x-api-path-slug: bucketsbucketkeyenvironments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
    post:
      summary: Add Buckets Environments
      description: Create new shared environment.
      operationId: buckets.bucketKey.environments.post
      x-api-path-slug: bucketsbucketkeyenvironments-post
      parameters:
      - in: body
        name: NewEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
  /buckets/{bucketKey}/environments/{environmentId}:
    put:
      summary: Put Buckets Environments
      description: Update the details of a shared environment.
      operationId: buckets.bucketKey.environments.environmentId.put
      x-api-path-slug: bucketsbucketkeyenvironmentsenvironmentid-put
      parameters:
      - in: body
        name: ModifiedEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Environments
  /buckets/{bucketKey}/errors:
    get:
      summary: Get Buckets Errors
      description: Retrieve a list of error messages in a bucket
      operationId: buckets.bucketKey.errors.get
      x-api-path-slug: bucketsbucketkeyerrors-get
      parameters:
      - in: query
        name: before
        description: Only return messages before the given Unix timestamp
      - in: query
        name: count
        description: Maxiumum number of messages to return
      - in: query
        name: No Name
      - in: query
        name: since
        description: Only return messages after the given Unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Errors
  /buckets/{bucketKey}/messages:
    delete:
      summary: Delete Buckets Messages
      description: Clear a bucket (remove all messages).
      operationId: buckets.bucketKey.messages.delete
      x-api-path-slug: bucketsbucketkeymessages-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
    get:
      summary: Get Buckets Messages
      description: Retrieve a list of messages in a bucket
      operationId: buckets.bucketKey.messages.get
      x-api-path-slug: bucketsbucketkeymessages-get
      parameters:
      - in: query
        name: before
        description: Only return messages before the given Unix timestamp
      - in: query
        name: count
        description: Maxiumum number of messages to return
      - in: query
        name: No Name
      - in: query
        name: since
        description: Only return messages after the given Unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
    post:
      summary: Add Buckets Messages
      description: Create a message
      operationId: buckets.bucketKey.messages.post
      x-api-path-slug: bucketsbucketkeymessages-post
      parameters:
      - in: body
        name: NewMessage
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Messages
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