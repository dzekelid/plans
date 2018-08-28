---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API Service Plan Create
  description: Service plan create.
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits.xml:
    get:
      summary: Limit List for End User Plans
      description: Limit list for end user plans .
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-get
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - ListEnd
      - User
      - Plans
    post:
      summary: Limit Create for End User Plans
      description: Limit create for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimits-xml-post
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - CreateEnd
      - User
      - Plans
  /admin/api/end_user_plans/{end_user_plan_id}/metrics/{metric_id}/limits/{id}.xml:
    delete:
      summary: Limit Delete for End User Plans
      description: Limit delete for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-delete
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
    get:
      summary: Limit Read for End User Plans
      description: Limit read for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-get
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - ReadEnd
      - User
      - Plans
    put:
      summary: Limit Update for End User Plans
      description: Limit update for end user plans.
      operationId: end_user_plan_limit
      x-api-path-slug: adminapiend-user-plansend-user-plan-idmetricsmetric-idlimitsid-xml-put
      parameters:
      - in: path
        name: end_user_plan_id
        description: id of the end user plan
      - in: path
        name: id
        description: id of the limit
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: period
        description: period of the limit
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: value
        description: value of the limit
      responses:
        200:
          description: OK
      tags:
      - Limit
      - End
      - User
      - Plans
  /admin/api/accounts/{account_id}/applications/{id}/change_plan.xml:
    put:
      summary: Application Change Plan
      description: Application change plan.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidchange-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: plan_id
        description: id of the new application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Change
      - Plan
  /admin/api/accounts/{account_id}/applications/{id}/customize_plan.xml:
    put:
      summary: Application Create Plan Customization
      description: Application create plan customization.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidcustomize-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Customization
  /admin/api/accounts/{account_id}/applications/{id}/decustomize_plan.xml:
    put:
      summary: Application Delete Plan Customization
      description: Application delete plan customization.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsiddecustomize-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - ""
      - Plan
      - Customization
  /admin/api/accounts/{account_id}/plan.xml:
    get:
      summary: Account Fetch Account Plan
      description: Account fetch account plan.
      operationId: account
      x-api-path-slug: adminapiaccountsaccount-idplan-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Fetch
      - Account
      - Plan
  /admin/api/accounts/{id}/change_plan.xml:
    put:
      summary: Account Change Plan
      description: Account change plan.
      operationId: account
      x-api-path-slug: adminapiaccountsidchange-plan-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: plan_id
        description: id of the target account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Change
      - Plan
  /admin/api/account_plans.xml:
    get:
      summary: Account Plan List
      description: Account plan list.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - List
    post:
      summary: Account Plan Create
      description: Account plan create.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Create
  /admin/api/account_plans/{account_plan_id}/features.xml:
    get:
      summary: Account Plan Feature List
      description: Account plan feature list.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Feature
      - List
  /admin/api/account_plans/{account_plan_id}/features/{id}.xml:
    delete:
      summary: Account Plan Features Delete
      description: Account plan features delete.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
    post:
      summary: Account Plan Features Create
      description: Account plan features create.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeaturesid-xml-post
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Features
      - Create
  /admin/api/account_plans/{id}.xml:
    delete:
      summary: Account Plan Delete
      description: Account plan delete.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
    get:
      summary: Account Plan Read
      description: Account plan read.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Read
    put:
      summary: Account Plan Update
      description: Account plan update.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: name
        description: Name of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
  /admin/api/account_plans/{id}/default.xml:
    put:
      summary: Account Plan set to Default
      description: Account plan set to default.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Set
      - To
      - Default
  /admin/api/application_plans.xml:
    get:
      summary: Application Plan List (all services)
      description: Application plan list (all services).
      operationId: application_plan
      x-api-path-slug: adminapiapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
      - (all
      - Services)
  /admin/api/application_plans/{application_plan_id}/features.xml:
    get:
      summary: Application Plan Feature List
      description: Application plan feature list.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
      - List
    post:
      summary: Application Plan Feature Create
      description: Application plan feature create.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-post
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: feature_id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
      - Create
  /admin/api/application_plans/{application_plan_id}/features/{id}.xml:
    delete:
      summary: Application Plan Feature Delete
      description: Application plan feature delete.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeaturesid-xml-delete
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
  /admin/api/application_plans/{application_plan_id}/limits.xml:
    get:
      summary: Limits List per Application Plan
      description: Limits list per application plan.
      operationId: application_plan_limits
      x-api-path-slug: adminapiapplication-plansapplication-plan-idlimits-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limits
      - List
      - Per
      - Application
      - Plan
  /admin/api/application_plans/{application_plan_id}/pricing_rules.xml:
    get:
      summary: Pricing Rules List per Application Plan
      description: Pricing rules list per application plan.
      operationId: application_plan_pricing_rules
      x-api-path-slug: adminapiapplication-plansapplication-plan-idpricing-rules-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Rules
      - List
      - Per
      - Application
      - Plan
  /admin/api/end_user_plans.xml:
    get:
      summary: End User Plan List (all services)
      description: End user plan list (all services).
      operationId: end_user_plan
      x-api-path-slug: adminapiend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
      - (all
      - Services)
  /admin/api/services/{id}/service_plans.xml:
    get:
      summary: Service Plan List
      description: Service plan list.
      operationId: service_plan
      x-api-path-slug: adminapiservicesidservice-plans-xml-get
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - List
    post:
      summary: Service Plan Create
      description: Service plan create.
      operationId: service_plan
      x-api-path-slug: adminapiservicesidservice-plans-xml-post
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: name
        description: Name of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Create
  /admin/api/services/{service_id}/application_plans.xml:
    get:
      summary: Application Plan List
      description: Application plan list.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
    post:
      summary: Application Plan Create
      description: Application plan create.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plans-xml-post
      parameters:
      - ~
      - in: query
        name: name
        description: Name of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: query
        name: system_name
        description: System Name of the object to be created
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Create
  /admin/api/services/{service_id}/application_plans/{id}.xml:
    delete:
      summary: Application Plan Delete
      description: Application plan delete.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
    get:
      summary: Application Plan Read
      description: Application plan read.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Read
    put:
      summary: Application Plan Update
      description: Application plan update.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansid-xml-put
      parameters:
      - ~
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: name
        description: Name of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
  /admin/api/services/{service_id}/application_plans/{id}/default.xml:
    put:
      summary: Application Plan set to Default
      description: Application plan set to default.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Set
      - To
      - Default
  /admin/api/services/{service_id}/end_users/{username}/change_plan.xml:
    put:
      summary: End User Change Plan
      description: End user change plan.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-usersusernamechange-plan-xml-put
      parameters:
      - in: query
        name: plan_id
        description: id of the new end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: path
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Change
      - Plan
  /admin/api/services/{service_id}/end_user_plans.xml:
    get:
      summary: End User Plan List
      description: End user plan list.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
    post:
      summary: End User Plan Create
      description: End user plan create.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plans-xml-post
      parameters:
      - in: query
        name: name
        description: Name of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Create
  /admin/api/services/{service_id}/end_user_plans/{id}.xml:
    get:
      summary: End User Plan Read
      description: End user plan read.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Read
    put:
      summary: End User Plan Update
      description: End user plan update.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: name
        description: Name of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
  /admin/api/services/{service_id}/end_user_plans/{id}/default.xml:
    put:
      summary: End User Plan set to Default
      description: End user plan set to default.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - Set
      - To
      - Default
  /admin/api/services/{service_id}/service_plans/{id}.xml:
    delete:
      summary: Service Plan Delete
      description: Service plan delete.
      operationId: service_plan
      x-api-path-slug: adminapiservicesservice-idservice-plansid-xml-delete
      parameters:
      - in: path
        name: id
        description: id of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
    get:
      summary: Service Plan Read
      description: Service plan read.
      operationId: service_plan
      x-api-path-slug: adminapiservicesservice-idservice-plansid-xml-get
      parameters:
      - in: path
        name: id
        description: id of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Read
    put:
      summary: Service Plan Update
      description: Service plan update.
      operationId: service_plan
      x-api-path-slug: adminapiservicesservice-idservice-plansid-xml-put
      parameters:
      - in: path
        name: id
        description: id of the service plan
      - in: query
        name: name
        description: Name of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
  /admin/api/services/{service_id}/service_plans/{id}/default.xml:
    put:
      summary: Service Plan set to Default
      description: Service plan set to default.
      operationId: service_plan
      x-api-path-slug: adminapiservicesservice-idservice-plansiddefault-xml-put
      parameters:
      - in: path
        name: id
        description: id of the service plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Set
      - To
      - Default
  /admin/api/service_plans.xml:
    get:
      summary: Service Plan List (all services)
      description: Service plan list (all services).
      operationId: service_plan
      x-api-path-slug: adminapiservice-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - List
      - (all
      - Services)
  /admin/api/service_plans/{service_plan_id}/features.xml:
    get:
      summary: Service Plan Feature List
      description: Service plan feature list.
      operationId: service_plan_feature
      x-api-path-slug: adminapiservice-plansservice-plan-idfeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_plan_id
        description: id of the service plan
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Feature
      - List
    post:
      summary: Service Plan Feature Add
      description: Service plan feature add.
      operationId: service_plan_feature
      x-api-path-slug: adminapiservice-plansservice-plan-idfeatures-xml-post
      parameters:
      - in: query
        name: feature_id
        description: id of the feature
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_plan_id
        description: id of the service plan
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Feature
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