{
  "info": {
    "name": "Easycron API Enable a cron job.",
    "_postman_id": "c4422244-ac9d-4dbe-b744-c80c065434c3",
    "description": "Enable a cron job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cron",
      "item": [
        {
          "id": "d21c28bf-e5ff-4b46-b577-6d4f79e2b414",
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
              "id": "52e620d4-64d6-4d80-a514-08baafa91920"
            }
          ]
        },
        {
          "id": "d8866a73-1b79-4991-9ed7-d2db1f808c53",
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
              "id": "14416651-e360-40de-a084-bbcc4395193a"
            }
          ]
        }
      ]
    },
    {
      "name": "Detail",
      "item": [
        {
          "id": "d85e887a-1d0e-4ccb-8527-aaecde9b7e20",
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
              "id": "103585d2-4abd-44f8-a2a3-899ed9ce71dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "9e6cc235-96a9-4248-8221-cdb849e7aad2",
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
              "id": "26654563-956a-47c0-81a9-e8ab04d87542"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "a952ab41-fb7d-4c94-b930-cd3411f9c56d",
          "name": "editCronJob",
          "request": {
            "url": "http://www.easycron.com/rest/edit?cookies=%7B%7D&cron_expression=%7B%7D&cron_job_name=%7B%7D&email_me=%7B%7D&id=%7B%7D&log_output_length=%7B%7D&posts=%7B%7D&testfirst=%7B%7D&token=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a cron job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb3edd0c-1d29-4a8e-b4d6-2cb4c1d85d0b"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "0568b3eb-7b9e-4802-9f88-d71d0c9697ee",
          "name": "enableCronJob",
          "request": {
            "url": "http://www.easycron.com/rest/enable?id=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enable a cron job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3429e8f-d824-46a0-be2c-555f86ecbdce"
            }
          ]
        }
      ]
    }
  ]
}