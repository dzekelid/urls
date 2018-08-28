swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/redirects/count.json:
    get:
      summary: Get a countt of all URL redirect
      description: Get a countt of all url redirect.
      operationId: getAdminRedirectsCount.json
      x-api-path-slug: adminredirectscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Countt
      - URL
      - Redirect
  /admin/redirects.json:
    get:
      summary: Get a list of all URL redirect
      description: Get a list of all url redirect.
      operationId: getAdminRedirects.json
      x-api-path-slug: adminredirects-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - URL
      - Redirect
  /admin/redirects/count/7376372.json:
    get:
      summary: Get a single URL redirect
      description: Get a single url redirect.
      operationId: getAdminRedirectsCount7376372.json
      x-api-path-slug: adminredirectscount7376372-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - URL
      - Redirect