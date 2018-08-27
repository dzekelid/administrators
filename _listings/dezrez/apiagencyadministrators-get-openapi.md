---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get the administrators for an agency
  version: 1.0.0
  description: Get the administrators for an agency.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branch/{id}/administrators:
    get:
      summary: Get Branch administrators by its id.
      description: Get branch administrators by its id..
      operationId: Branch_AdministratorsByid
      x-api-path-slug: apibranchidadministrators-get
      parameters:
      - in: path
        name: id
        description: The id of the Branch administrators to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Branch
      - Administrators
      - By
      - Its
      - Id
  /api/agency/administrators:
    get:
      summary: Get the administrators for an agency
      description: Get the administrators for an agency.
      operationId: Agency_Administrators
      x-api-path-slug: apiagencyadministrators-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Administratorsan
      - Agency
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