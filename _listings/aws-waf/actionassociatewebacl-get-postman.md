{
  "info": {
    "name": "AWS WAF API Associate Web ACL",
    "_postman_id": "eb9b11ac-b348-4862-898f-edea8a41a25f",
    "description": "Service: AWS WAF RegionalAssociates a web ACL with a resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "40a81623-a363-4f7e-b7ea-48b03bfc62eb",
          "name": "associateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=AssociateWebACL?ResourceArn=ResourceArn&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalAssociates a web ACL with a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a63a2071-76db-4ad1-9b33-4b9227d51d04"
            }
          ]
        }
      ]
    }
  ]
}