{
  "info": {
    "name": "Transportation Laws and Incentives Return a full list of laws and incentives that match your query.",
    "_postman_id": "451aedb0-c8bb-43de-88c2-d7d07b7f34cb",
    "description": "Return a full list of laws and incentives that match your query..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Return",
      "item": [
        {
          "id": "b218211f-733e-46d5-95ed-4d455e8e8406",
          "name": "v1.output_format.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "transportation-incentives-laws",
                "v1.:output_format"
              ],
              "query": [
                {
                  "key": "expired",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "incentive_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "jurisdiction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "keyword",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "law_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "local",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "recent",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "regulation_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "technology",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_format",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a full list of laws and incentives that match your query.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "998e8fb2-5e16-4a0e-bb83-74d57bef090c"
            }
          ]
        }
      ]
    }
  ]
}