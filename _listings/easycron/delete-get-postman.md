{
  "info": {
    "name": "Easycron API Delete a cron job.",
    "_postman_id": "8cf9fc0c-9fe2-41ad-a915-33d4f8fdf929",
    "description": "Delete a cron job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cron",
      "item": [
        {
          "id": "1bc52d7c-3d04-4152-be99-903adbc9a8b9",
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
              "id": "2a96744f-9c74-4822-b543-364b33b772e4"
            }
          ]
        },
        {
          "id": "76c3d39e-ac64-4c1a-b5e6-7c556e3e6ef5",
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
              "id": "2a7b26b4-4fe9-438c-b57d-2cf5393575ee"
            }
          ]
        }
      ]
    }
  ]
}