{
  "info": {
    "name": "Runscope Get Buckets",
    "_postman_id": "d18f3e1f-717e-443a-8251-02c05350ab29",
    "description": "Returns a list of buckets.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "f5b07dc2-b1b2-408f-ab84-f074aa204af0",
          "name": "buckets.get",
          "request": {
            "url": "http://api.runscope.com/buckets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of buckets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d42c0f0-e64f-4222-9ce2-73b38928497a"
            }
          ]
        }
      ]
    }
  ]
}