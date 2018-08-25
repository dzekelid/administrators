---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
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
---