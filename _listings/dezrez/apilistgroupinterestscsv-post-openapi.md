---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a csv file from selected group interest list items
  version: 1.0.0
  description: Generates a csv file from selected group interest list items.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/batchpaymentcsv:
    post:
      summary: Get details formatted for batch payment csv
      description: Get details formatted for batch payment csv.
      operationId: AccountingExport_ExportBatchPaymentBydataContract
      x-api-path-slug: apiaccountingexportsbatchpaymentcsv-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Details
      - Formattedbatch
      - Payment
      - Csv
  /api/accounting/exports/ledgerentriescsv:
    post:
      summary: Get ledger items formatted for export csv
      description: Get ledger items formatted for export csv.
      operationId: AccountingExport_ExportLedgerEntriesCsvBydataContract
      x-api-path-slug: apiaccountingexportsledgerentriescsv-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Ledger
      - Items
      - Formattedexport
      - Csv
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
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