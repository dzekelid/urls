---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Statistics Get Chart Url Custom
  description: Get chart url for a topic.
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ', Url':
    get:
      summary: Get Chart Url
      description: Get chart url for a topic.
      operationId: postGetcharturl
      x-api-path-slug: url-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Url
  ', Url, Preset':
    get:
      summary: Get Chart Url Preset
      description: Get chart url for a topic.
      operationId: postGetcharturlpreset
      x-api-path-slug: url-preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Url
      - Preset
  ', Url, Custom':
    get:
      summary: Get Chart Url Custom
      description: Get chart url for a topic.
      operationId: postGetcharturlcustom
      x-api-path-slug: url-custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Url
      - Custom
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