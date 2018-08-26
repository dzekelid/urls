---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Set base url
  description: Sets the base URL that is configured for this Jira instance.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/settings/baseUrl:
    put:
      summary: Set base url
      description: Sets the base URL that is configured for this Jira instance.
      operationId: com.atlassian.jira.rest.v2.admin.SettingsResource.setBaseURL_put
      x-api-path-slug: api2settingsbaseurl-put
      responses:
        200:
          description: OK
      tags:
      - Set
      - Base
      - Url
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