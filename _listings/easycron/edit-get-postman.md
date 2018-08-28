{
  "info": {
    "name": "Easycron API Edit a cron job.",
    "_postman_id": "22bb9e88-ce14-406c-a538-37ec0905cb84",
    "description": "Edit a cron job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cron",
      "item": [
        {
          "id": "846fd1d6-302b-42f7-9a85-6cee2192bd7a",
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
              "id": "00853ce0-e249-4466-b72a-2c82e38be485"
            }
          ]
        },
        {
          "id": "329fffd0-47e1-43e6-921c-9fee85f06cac",
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
              "id": "78e42c04-19a5-4c90-a43e-ea4bbe03b746"
            }
          ]
        }
      ]
    },
    {
      "name": "Detail",
      "item": [
        {
          "id": "a29487c4-e839-4607-ba6d-34916df189ff",
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
              "id": "0d79ff84-e293-43ea-9298-51e3e47a7e41"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "8abf45d2-685e-4ebf-b70a-59ee699189de",
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
              "id": "e0b4e174-7451-4a9d-90ab-40962de24975"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "8b5d2578-7526-4618-ba02-ba041b6a00df",
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
              "id": "17aacfdf-14b4-4656-a6f8-0c130a3800de"
            }
          ]
        }
      ]
    }
  ]
}