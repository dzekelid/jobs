{
  "info": {
    "name": "Easycron API Disable a cron job",
    "_postman_id": "d13aba2a-524f-4f62-af5d-8f3b26610a18",
    "description": "Disable a cron job",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cron",
      "item": [
        {
          "id": "0d7d9076-6e9b-45b8-9eeb-76aaf29ba9bc",
          "name": "addCronJob",
          "request": {
            "url": "http://www.easycron.com/rest/add?cookies=%7B%7D&cron_expression=%7B%7D&cron_job_name=%7B%7D&email_me=%7B%7D&log_output_length=%7B%7D&posts=%7B%7D&testfirst=%7B%7D&token=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add a cron job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "689da73f-64d5-49b7-8521-5ca2ccc0c993"
            }
          ]
        },
        {
          "id": "5b4eb610-ca4a-4edc-8ebf-3922aaf0f63a",
          "name": "deleteCronJob",
          "request": {
            "url": "http://www.easycron.com/rest/delete?id=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a cron job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49977227-eff8-4d01-9b9d-10bf3004af33"
            }
          ]
        }
      ]
    },
    {
      "name": "Detail",
      "item": [
        {
          "id": "e5744fbf-5f09-421b-b53b-8e75160a82c9",
          "name": "getDetailCronJob",
          "request": {
            "url": "http://www.easycron.com/rest/detail?id=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detail of a cron job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0aac98d8-6578-4221-816d-7041b50fc703"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "853d14c1-a9f3-4c72-a31f-619b3da90f5f",
          "name": "disableCronJbo",
          "request": {
            "url": "http://www.easycron.com/rest/disable?id=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disable a cron job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0d3da94-07ba-473e-828f-231a4a4f3668"
            }
          ]
        }
      ]
    }
  ]
}