---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve a plan
  description: Retrieve a plan with specified identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /plans:
    get:
      summary: Retrieve a list of plans
      description: Retrieve a list of plans
      operationId: plans.get
      x-api-path-slug: plans-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Plans
    post:
      summary: Create a plan
      description: Create a plan
      operationId: plans.post
      x-api-path-slug: plans-post
      parameters:
      - in: body
        name: body
        description: Plan resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Plan
  /plans/{id}:
    delete:
      summary: Delete a Plan
      description: Delete a Plan with predefined identifier string
      operationId: plans.id.delete
      x-api-path-slug: plansid-delete
      responses:
        200:
          description: OK
      tags:
      - Plan
    get:
      summary: Retrieve a plan
      description: Retrieve a plan with specified identifier string
      operationId: plans.id.get
      x-api-path-slug: plansid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Plan
    put:
      summary: Create or update a Plan with predefined ID
      description: Create or update a Plan with predefined identifier string
      operationId: plans.id.put
      x-api-path-slug: plansid-put
      parameters:
      - in: body
        name: body
        description: Plan resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Plan
      - Predefined
      - ID
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