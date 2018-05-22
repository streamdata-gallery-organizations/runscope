{
  "info": {
    "name": "Runscope Get Buckets Tests Steps",
    "_postman_id": "4e706b2d-f3cf-425c-81cf-b4c5d14e13f9",
    "description": "List test steps for a test.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "151a9ed6-de63-4ab2-9a50-0adaf0f958d3",
          "name": "buckets.bucketKey.tests.testId.steps.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests/:testId/steps"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "bucketKey",
                  "value": "bucketKey",
                  "type": "string"
                },
                {
                  "id": "testId",
                  "value": "testId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List test steps for a test"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4e7a169-3218-4083-a6ad-aaeb5ff44716"
            }
          ]
        }
      ]
    }
  ]
}