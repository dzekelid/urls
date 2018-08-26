---
swagger: "2.0"
x-collection-name: Apica
x-complete: 0
info:
  title: Checks URL Checks URL Locations
  version: 1.0.0
  description: Gets a list of all locations that are available for URL (version 2)
    checks.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/checks/url ':
    ' post ':
      summary: Checks URL
      description: Creates a new URL check (legacy version 1).
      operationId: -checks-url-
      x-api-path-slug: checksurl-post
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
  '/checks/url-v2 ':
    ' post ':
      summary: Checks URL
      description: Creates a new URL check (version 2).
      operationId: -checks-url-v2-
      x-api-path-slug: checksurlv2-post
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
  '/checks/url/{checkId} ':
    ' put ':
      summary: Checks URL
      description: Updates a URL check (legacy version 1).
      operationId: -checks-url-checkid-
      x-api-path-slug: checksurlcheckid-put
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
  '/checks/url-v2/{checkId} ':
    ' put ':
      summary: Checks URL
      description: Updates a URL check (version 2).
      operationId: -checks-url-v2-checkid-
      x-api-path-slug: checksurlv2checkid-put
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
  '/checks/url/locations ':
    ' get ':
      summary: Checks URL Locations
      description: Gets a list of all locations that are available for URL (legacy
        version 1) checks.
      operationId: -checks-url-locations-
      x-api-path-slug: checksurllocations-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
  '/checks/url-v2/locations ':
    ' get ':
      summary: Checks URL Locations
      description: Gets a list of all locations that are available for URL (version
        2) checks.
      operationId: -checks-url-v2-locations-
      x-api-path-slug: checksurlv2locations-get
      responses:
        200:
          description: OK
      tags:
      - Checks
      - URL
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