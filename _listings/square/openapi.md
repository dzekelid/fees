---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/fees:
    get:
      summary: Lists all of a location's fees (taxes).
      description: Lists all of a location's fees (taxes).
      operationId: ListFees
      x-api-path-slug: v1location-idfees-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list fees for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Fees
      - (taxes)
  /v1/{location_id}/items/{item_id}:
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
---