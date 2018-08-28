{
  "info": {
    "name": "Easycron API Add a cron job.",
    "_postman_id": "5f0e719f-ef51-4eba-8539-2837f8725b1f",
    "description": "Add a cron job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cron",
      "item": [
        {
          "id": "0d217ae3-d71d-4ead-bf67-c989c05364f1",
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
              "id": "8919a7a4-2696-4601-a480-0d7c4f2b67c4"
            }
          ]
        }
      ]
    }
  ]
}