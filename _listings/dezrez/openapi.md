---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ExternalProvider:
    get:
      summary: Returns a URL that will start the process of authorisation with the
        external provider - normally using the OAuth1/2 protocol suite.
      description: Returns a url that will start the process of authorisation with
        the external provider - normally using the oauth1/2 protocol suite..
      operationId: ExternalProvider_GetAuthoriseAgencyUrlByexternalProviderId
      x-api-path-slug: apiexternalprovider-get
      parameters:
      - in: query
        name: externalProviderId
        description: The external provider identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - URL
      - That
      - Will
      - Start
      - Process
      - Of
      - Authorisation
      - External
      - Provider
      - '-'
      - Normally
      - Using
      - OAuth1
      - "2"
      - Protocol
      - Suite
---