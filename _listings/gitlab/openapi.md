swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/internal/merge_request_urls:
    get:
      summary: Get Internal Merge Request Urls
      description: Get internal merge request urls.
      operationId: getV3InternalMergeRequestUrls
      x-api-path-slug: v3internalmerge-request-urls-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Merge
      - Request
      - Urls