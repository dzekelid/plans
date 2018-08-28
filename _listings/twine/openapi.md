swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
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