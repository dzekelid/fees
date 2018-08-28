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
  /api/fee/getall:
    get:
      summary: Get list of all fees stored
      description: Get list of all fees stored.
      operationId: Fee_GetFeesBypageSizeBypageNumber
      x-api-path-slug: apifeegetall-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Fees
      - Stored
  /api/invoice/fees:
    get:
      summary: Get agent fees invoices earned
      description: Get agent fees invoices earned.
      operationId: Invoice_GetAgentFeesEarned
      x-api-path-slug: apiinvoicefees-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Agent
      - Fees
      - Invoices
      - Earned