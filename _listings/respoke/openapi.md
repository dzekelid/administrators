swagger: "2.0"
x-collection-name: Respoke
x-complete: 1
info:
  title: Respoke REST API
  description: add-live-voice-video-text-and-data-features-to-your-website-or-app-
  termsOfService: https://www.respoke.io/files/respoke-tos-20141007.pdf
  version: v1
host: api.respoke.io
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  adminsessions/:
    post:
      summary: Permissions
      description: Full API permissions are obtained by POSTing your username and
        password to [base]/adminsessions.
      operationId: postAdminsessions
      x-api-path-slug: adminsessions-post
      parameters:
      - in: query
        name: password
        description: Your username
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Adminsessions