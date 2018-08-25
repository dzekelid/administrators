---
swagger: "2.0"
x-collection-name: Strava
x-complete: 1
info:
  title: Strava API v3
  description: strava-api
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clubs/{id}/admins:
    get:
      summary: List Club Administrators.
      description: Returns a list of the administrators of a given club.
      operationId: getClubAdminsById
      x-api-path-slug: clubsidadmins-get
      parameters:
      - in: path
        name: id
        description: The identifier of the club
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Club
      - Administrators
---