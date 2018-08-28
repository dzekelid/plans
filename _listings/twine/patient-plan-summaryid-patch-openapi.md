---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Update a plan summary
  description: Update a plan summary record for a patient.
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /patient_plan_summary:
    get:
      summary: List patient plan summaries
      description: Get a list of patient plan summaries
      operationId: fetchPatientPlanSummaries
      x-api-path-slug: patient-plan-summary-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient id to fetch plan summary for
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Patient
      - Plan
      - Summaries
  /patient_plan_summary/{id}:
    get:
      summary: Get the plan summary for a patient
      description: Get the plan summary for a patient.
      operationId: fetchPatientPlanSummary
      x-api-path-slug: patient-plan-summaryid-get
      parameters:
      - in: path
        name: id
        description: Plan summary identifier
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Plan
      - Summarya
      - Patient
    patch:
      summary: Update a plan summary
      description: Update a plan summary record for a patient.
      operationId: updatePatientPlanSummary
      x-api-path-slug: patient-plan-summaryid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Plan summary identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Plan
      - Summary
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