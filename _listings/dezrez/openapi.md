---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
---