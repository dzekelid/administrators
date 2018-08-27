---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets project group admins
  version: 1.0.0
  description: Gets project group admins.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectid}/admins:
    get:
      summary: Gets project administrators
      description: Gets project administrators.
      operationId: getProjectAdmins
      x-api-path-slug: projectsprojectidadmins-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Administrators
  /projectgroups/{projectgroupid}/admins:
    get:
      summary: Gets project group admins
      description: Gets project group admins.
      operationId: getProjectGroupAdmins
      x-api-path-slug: projectgroupsprojectgroupidadmins-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Admins
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