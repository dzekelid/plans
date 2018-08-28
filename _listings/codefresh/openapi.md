swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /payments/plans:
    get:
      summary: Get Payments Plans
      description: Get payments plans.
      operationId: getPaymentsPlans
      x-api-path-slug: paymentsplans-get
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Plans