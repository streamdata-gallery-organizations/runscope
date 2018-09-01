{
  "info": {
    "name": "Runscope Put Buckets Tests",
    "_postman_id": "efaf51e8-f9bb-40f8-9efa-c5bca1b11af2",
    "description": "Modify a test's name, description, default environment and its steps. To modify other individual properties of a test, make requests to the steps, environments, and schedules subresources of the test.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "3d88da90-85b1-4b8c-a179-830c9283206d",
          "name": "buckets.bucketKey.tests.testId.put",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a test's name, description, default environment and its steps"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99c3a413-2175-42f8-9b84-22dbdf298c2c"
            }
          ]
        }
      ]
    }
  ]
}