---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns a list of customer booking limits.
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/customers/plans:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersPlansGet
      x-api-path-slug: consumerv1customersplans-get
      parameters:
      - in: query
        name: groupId
        description: Filter customers by group
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Plans
  /consumer/v1/customers/plans/{id}:
    get:
      summary: Returns a customer object.
      description: "The result returned is a single customer object. An id is required
        to find the customer. Find customer id's using either the GET consumer/v1/customers
        end point,\r\nor the GET consumer/v1/appointments end point. A customer object
        is automatically created with the first booking if it doesn't already exist."
      operationId: ConsumerV1CustomersPlansByIdGet
      x-api-path-slug: consumerv1customersplansid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Plans
  /consumer/v1/customers/{id}/planlimits/{serviceId}/{resourceId}/{dateTimeTz}:
    get:
      summary: Returns a list of customer booking limits.
      description: "The result returned is list of limit rules as defined by the subscribed
        customer plan along with Booking Counts/Minutes\r\nThe results indicate the
        remaining bookings count / minutes. Use the results in your app to determine
        if the customer should continue booking.\r\nYou can enforce Limits in periods:
        Daily,Weekly,Monthly and for maximum total limits. Maximum total limits is
        based on six months prior to\r\nthe DateTimeTz and six months after the DateTimeTz.
        Daily, Weekly and Monthly limits are based on the calculated period relative
        to the\r\nsubscription plan start. Daily,Weekly and Monthly limits can be
        setup on a per interval basis e.g. to biweekly, or daily every 10 days.\r\nSee
        customer plans setup in the Portal for more information.\r\nAll parameters
        are required. If resourceId is not applicable for a non-resource calendar,
        pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
      operationId: ConsumerV1CustomersByIdPlanlimitsByServiceIdByResourceIdByDateTimeTzGet
      x-api-path-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
      parameters:
      - in: path
        name: dateTimeTz
        description: The DateTimeTz to check
      - in: path
        name: id
        description: The id of the customer object
      - in: path
        name: resourceId
        description: The id of the resource object
      - in: path
        name: serviceId
        description: The id of the service object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Planlimits
      - ServiceId
      - ResourceId
      - DateTimeTz
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