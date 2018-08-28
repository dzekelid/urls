---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get file information for a single object in frontend storage.
    Append public cloudfront url to retrieved object.
  description: Get file information for a single object in frontend storage. append
    public cloudfront url to retrieved object..
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
  /rest/accounts/contacts/{contactId}/access_data/login_url:
    get:
      summary: Get the login URL
      description: Gets the URL to login as the given contact. The ID of the contact
        must be specified.
      operationId: getRestAccountsContactsContactAccessDataLoginUrl
      x-api-path-slug: restaccountscontactscontactidaccess-datalogin-url-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Login
      - URL
  /rest/markets/ebay/auth/login:
    get:
      summary: Get the login url.
      description: Get the login url..
      operationId: getRestMarketsEbayAuthLogin
      x-api-path-slug: restmarketsebayauthlogin-get
      responses:
        200:
          description: OK
      tags:
      - Login
      - Url
  /rest/storage/frontend/file:
    get:
      summary: Get file information for a single object in frontend storage. Append
        public cloudfront url to retrieved object.
      description: Get file information for a single object in frontend storage. append
        public cloudfront url to retrieved object..
      operationId: getRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-get
      parameters:
      - in: query
        name: key
        description: The key of the object to get information about
      responses:
        200:
          description: OK
      tags:
      - File
      - Informationa
      - Single
      - Object
      - In
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Retrieved
      - Object
  /rest/storage/frontend/files:
    get:
      summary: List files from frontend storage. Append public cloudfront url to each
        retrieved object.
      description: List files from frontend storage. append public cloudfront url
        to each retrieved object..
      operationId: getRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-get
      parameters:
      - in: query
        name: continuationToken
        description: The continuationToken of a previous request to continue listing
          objects with
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Each
      - Retrieved
      - Object
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