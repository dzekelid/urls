---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/products/{productId}/generateApprovalUrl:
    post:
      summary: Generates a URL
      description: |-
        Generates a URL that can be rendered in an iframe to display the permissions (if any) of a product. An enterprise admin must view these permissions and accept them on behalf of their organization in order to approve that product.

        Admins should accept the displayed permissions by interacting with a separate UI element in the EMM console, which in turn should trigger the use of this URL as the approvalUrlInfo.approvalUrl property in a Products.approve call to approve the product. This URL can only be used to display permissions for up to 1 day.
      operationId: androidenterprise.products.generateApprovalUrl
      x-api-path-slug: enterprisesenterpriseidproductsproductidgenerateapprovalurl-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: languageCode
        description: The BCP 47 language code used for permission names and descriptions
          in the returned iframe, for instance en-US
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - URL
---