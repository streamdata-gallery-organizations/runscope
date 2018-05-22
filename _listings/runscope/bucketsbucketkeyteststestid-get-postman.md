{
  "info": {
    "name": "Runscope Get Buckets Tests",
    "_postman_id": "1f5a384f-e1c0-4f38-b064-6af79913f05b",
    "description": "Retrieve the details of a given test by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "3b108bc9-ac31-44da-a79d-f42eead86de4",
          "name": "buckets.bucketKey.tests.testId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests/:testId"
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
            "description": "Retrieve the details of a given test by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c2af8d-ac40-4ff4-8cab-b78d0624f328"
            }
          ]
        }
      ]
    }
  ]
}