---
swagger: "2.0"
x-collection-name: EasyCron
x-complete: 0
info:
  title: Easycron API Get detail of a cron job.
  description: Get detail of a cron job.
  termsOfService: https://www.easycron.com/terms
  contact:
    name: EasyCron
    url: https://www.easycron.com/contact
  version: 1.0.0
host: www.easycron.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /add:
    get:
      summary: Add a cron job.
      description: Add a cron job.
      operationId: addCronJob
      x-api-path-slug: add-get
      parameters:
      - in: query
        name: cookies
        description: Cookie variable-value pairs
      - in: query
        name: cron_expression
        description: Cron expression that following the syntax defined at our Cron
          Expression page
      - in: query
        name: cron_job_name
        description: The name of your cron job
      - in: query
        name: email_me
        description: Email notification setting of the cron job
      - in: query
        name: log_output_length
        description: Length of execution log of the cron job
      - in: query
        name: posts
        description: POST variable-value pairs
      - in: query
        name: testfirst
        description: If to test the cron job URL first before adding
      - in: query
        name: token
        description: You API token
      - in: query
        name: url
        description: URL of the cron job
      responses:
        200:
          description: OK
      tags:
      - Cron
      - Job
  /delete:
    get:
      summary: Delete a cron job.
      description: Delete a cron job.
      operationId: deleteCronJob
      x-api-path-slug: delete-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to delete
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Cron
      - Job
  /detail:
    get:
      summary: Get detail of a cron job.
      description: Get detail of a cron job.
      operationId: getDetailCronJob
      x-api-path-slug: detail-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to get detail of
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Detail
      - Of
      - Cron
      - Job
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---