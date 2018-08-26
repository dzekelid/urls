---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get the URL for a order property file
  description: |-
    Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
    minutes.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/document/url:
    get:
      summary: Get a temporary url for a single document
      description: Get a temporary url for a single document.
      operationId: getRestAccountsContactsContactDocumentUrl
      x-api-path-slug: restaccountscontactscontactiddocumenturl-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key to get temporary url for
      responses:
        200:
          description: OK
      tags:
      - Temporary
      - Urla
      - Single
      - Document
  /rest/storage/frontend/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageFrontendObjectUrl
      x-api-path-slug: reststoragefrontendobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the frontend document to retrieve the URL
          for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
  /rest/storage/layout/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageLayoutObjectUrl
      x-api-path-slug: reststoragelayoutobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
  /rest/storage/order-properties/object-url:
    get:
      summary: Get the URL for a order property file
      description: |-
        Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
        minutes.
      operationId: getRestStorageOrderPropertiesObjectUrl
      x-api-path-slug: reststorageorderpropertiesobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the order property     *                        file
          to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Order
      - Property
      - File
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