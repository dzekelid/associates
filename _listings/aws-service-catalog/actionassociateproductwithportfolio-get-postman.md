{
  "info": {
    "name": "AWS Service Catalog API Associate Product With Portfolio",
    "_postman_id": "18ebf203-a61f-4425-8377-a19d3b3cc18b",
    "description": "Associates a product with a portfolio.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Portfolios",
      "item": [
        {
          "id": "e726ca09-e7f5-4ba4-956e-27685390bb5e",
          "name": "acceptPortfolioShare",
          "request": {
            "url": "http://example.com/api/?Action=AcceptPortfolioShare?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts an offer to share a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e91cb73-ee29-4f67-b76e-bf8727d9f89b"
            }
          ]
        },
        {
          "id": "78a536d4-659f-4ce8-88f7-3c3e359e961e",
          "name": "associatePrincipalWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociatePrincipalWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&PrincipalARN=PrincipalARN&PrincipalType=PrincipalType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified principal ARN with the specified portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c94b7bc-aff7-4183-bd5d-29e69e6b5768"
            }
          ]
        },
        {
          "id": "e79243c9-57a6-443f-ae13-06b52edecc91",
          "name": "associateProductWithPortfolio",
          "request": {
            "url": "http://example.com/api/?Action=AssociateProductWithPortfolio?AcceptLanguage=AcceptLanguage&PortfolioId=PortfolioId&ProductId=ProductId&SourcePortfolioId=SourcePortfolioId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a product with a portfolio."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e673faf3-d41d-405d-bb7e-0bf698a0d409"
            }
          ]
        }
      ]
    }
  ]
}