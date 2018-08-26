---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/CustomerGroups:
    put:
      summary: This method updates a collection of customer groups in the database.
        No URL parameters should be included.
      description: This method updates a collection of customer groups in the database.
        no url parameters should be included..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroups-put
      parameters:
      - in: body
        name: customergroups
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Updates
      - Collection
      - Of
      - Customer
      - Groups
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Customers:
    put:
      summary: This method is used to update multiple customers in the system. No
        URL parameters should be included.
      description: This method is used to update multiple customers in the system.
        no url parameters should be included..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customers-put
      parameters:
      - in: body
        name: customers
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Customers
      - In
      - System
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Manufacturers:
    put:
      summary: This method is used to update multiple manufacturers in the database.
        No URL parameters should be included.
      description: This method is used to update multiple manufacturers in the database.
        no url parameters should be included..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturers-put
      parameters:
      - in: body
        name: manufacturers
        description: A Json or XML object containing the new manufacturers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Manufacturers
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Orders:
    put:
      summary: This method is used to update multiple orders in the database. No URL
        parameters should be included.
      description: This method is used to update multiple orders in the database.
        no url parameters should be included..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1orders-put
      parameters:
      - in: body
        name: orders
        description: A Json or XML object containing the orders
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Orders
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/PaymentTokens:
    put:
      summary: This method is used to update multiple paymenttokens in the database.
        No URL parameters should be included.
      description: This method is used to update multiple paymenttokens in the database.
        no url parameters should be included..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokens-put
      parameters:
      - in: body
        name: paymenttokens
        description: A Json or XML object containing the new PaymentTokens
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Paymenttokens
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Products:
    put:
      summary: This method is used to update multiple products in the database. No
        URL parameters should be included.
      description: This method is used to update multiple products in the database.
        no url parameters should be included..
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1products-put
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: products
        description: A Json or XML object containing the new product(s)
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Products
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
---