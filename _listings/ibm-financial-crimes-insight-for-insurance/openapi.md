swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/account/{id}:
    get:
      summary: Retrieve account data from the database, for the id
      description: This method is used to retrieve account data from the database
      operationId: getAccount
      x-api-path-slug: ibmfciplatformfactaccountid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Account
      - Data
      - From
      - Database
      - The
      - Id
  /ibm/fci/platform/fact/account:
    put:
      summary: Insert account data into the database
      description: This method is used to insert account data into the database.  The
        XML schema is defined in the ACCOUNT.XSD file.
      operationId: putAccount
      x-api-path-slug: ibmfciplatformfactaccount-put
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Account
      - Data
      - Into
      - Database