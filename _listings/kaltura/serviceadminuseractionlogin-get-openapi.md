---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Adminuser Action Login
  description: Get an admin session using admin email and password (Used for login
    to the KMC application)
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/adminuser/action/login:
    get:
      summary: Get Service Adminuser Action Login
      description: Get an admin session using admin email and password (Used for login
        to the KMC application)
      operationId: adminUser.login
      x-api-path-slug: serviceadminuseractionlogin-get
      parameters:
      - in: query
        name: email
      - in: query
        name: No Name
      - in: query
        name: partnerId
      - in: query
        name: password
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - Login
  /service/adminuser/action/resetPassword:
    get:
      summary: Get Service Adminuser Action Resetpassword
      description: Reset admin user password and send it to the users email address
      operationId: adminUser.resetPassword
      x-api-path-slug: serviceadminuseractionresetpassword-get
      parameters:
      - in: query
        name: email
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - ResetPassword
  /service/adminuser/action/setInitialPassword:
    get:
      summary: Get Service Adminuser Action Setinitialpassword
      description: Set initial users password
      operationId: adminUser.setInitialPassword
      x-api-path-slug: serviceadminuseractionsetinitialpassword-get
      parameters:
      - in: query
        name: hashKey
      - in: query
        name: newPassword
        description: new password to set
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - SetInitialPassword
  /service/adminuser/action/updatePassword:
    get:
      summary: Get Service Adminuser Action Updatepassword
      description: Update admin user password and email
      operationId: adminUser.updatePassword
      x-api-path-slug: serviceadminuseractionupdatepassword-get
      parameters:
      - in: query
        name: email
      - in: query
        name: newEmail
        description: Optional, provide only when you want to update the email
      - in: query
        name: newPassword
      - in: query
        name: No Name
      - in: query
        name: password
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - UpdatePassword
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