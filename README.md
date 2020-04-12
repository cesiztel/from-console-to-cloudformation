# From AWS Management Console to Cloudformation

Welcome to my way to support the AWS community. I hope this project help you in your journey using AWS services. AWS team is always great creating new content in their [blog](https://aws.amazon.com/blogs). There are many articles that solve real-life project problems, but they are using AWS Management Console. Do not get me wrong!. I understand that this articles are oriented for the general public, but in many companies, this is not the way we work. Cloudformation is the most susteinable solution for many teams to deploy and maintain their services. With the goal of help the community, I am trying to translate official AWS blog posts in Cloudformation templates, ready to deploy. 

## List of articles

### Compute blog

Official site: https://aws.amazon.com/blogs/compute/

#### Articles

- Using Amazon API Gateway as a proxy for DynamoDB

  Official link: https://aws.amazon.com/blogs/compute/using-amazon-api-gateway-as-a-proxy-for-dynamodb/
  
  CloudFormation templates:
  * [Main folder](/apigateway-proxy-dynamodb)
  * [Create the DynamoDB stack](/apigateway-proxy-dynamodb/dynamodb-template.yml)
  * [Create the ApiGateway stack](/apigateway-proxy-dynamodb/apigateway-template.yml)
  Notes: 
  For the ApiGateway you will need create a role with access to actions in DynamoDB. You
  can add it's ARN as value of the parameter `DynamoDBRoleARN`