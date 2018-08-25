{
  "info": {
    "name": "AWS Service Catalog API Associate Principal With Portfolio",
    "_postman_id": "a5deb556-1989-4655-8909-5ee295ad7c1b",
    "description": "Associates the specified principal ARN with the specified portfolio.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Portfolios",
      "item": [
        {
          "id": "6f486ce9-81e1-418f-8d95-8b758eb13e52",
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
              "id": "8af314f1-8ec5-4810-a9fe-3c3418de7203"
            }
          ]
        },
        {
          "id": "e13a8651-3078-4d76-8a5a-eb4d9713a55d",
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
              "id": "7bc40c25-4698-4a55-89c5-e28611b4ac14"
            }
          ]
        }
      ]
    }
  ]
}