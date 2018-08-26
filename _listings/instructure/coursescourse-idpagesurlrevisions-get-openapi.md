---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List revisions
  description: List revisions.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/pages/url:
    delete:
      summary: Delete page
      description: Delete page.
      operationId: delete-page
      x-api-path-slug: coursescourse-idpagesurl-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
    get:
      summary: Show page
      description: Show page.
      operationId: show-page
      x-api-path-slug: coursescourse-idpagesurl-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
    put:
      summary: Update/create page
      description: Update/create page.
      operationId: updatecreate-page
      x-api-path-slug: coursescourse-idpagesurl-put
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[front_page]
        description: Set an unhidden page as the front page (if true)
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
  /courses/{course_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: coursescourse-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
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