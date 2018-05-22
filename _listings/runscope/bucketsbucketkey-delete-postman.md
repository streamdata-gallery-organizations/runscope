{
  "info": {
    "name": "Runscope Delete Buckets Bucketkey",
    "_postman_id": "70b193d8-f9ff-47af-a853-d7e57016fc92",
    "description": "Delete a single bucket resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "321d389c-0fe4-4d5a-9022-b9725b16936b",
          "name": "buckets.bucketKey.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey"
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
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a single bucket resource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3b0a570-e395-4669-95ab-beb8055dec35"
            }
          ]
        }
      ]
    }
  ]
}