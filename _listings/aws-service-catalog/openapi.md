---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociatePrincipalWithPortfolio:
    get:
      summary: Associate Principal With Portfolio
      description: Associates the specified principal ARN with the specified portfolio.
      operationId: associatePrincipalWithPortfolio
      x-api-path-slug: actionassociateprincipalwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      - in: query
        name: PrincipalType
        description: The principal type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=AssociateProductWithPortfolio:
    get:
      summary: Associate Product With Portfolio
      description: Associates a product with a portfolio.
      operationId: associateProductWithPortfolio
      x-api-path-slug: actionassociateproductwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: SourcePortfolioId
        description: The identifier of the source portfolio to use with this association
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
---