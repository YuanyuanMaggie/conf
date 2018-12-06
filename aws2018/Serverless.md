# Serverless on AWS

## Serverless web application

![Web Application Architecture](https://github.com/aws-samples/aws-serverless-workshops/blob/master/WebApplication/images/wildrydes-complete-architecture.png)

- Web host: [Amazon S3](https://aws.amazon.com/s3/). S3 hosts static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser. 
- Auth: [Amazon Cognito](https://aws.amazon.com/cognito/). Amazon Cognito provides user management and authentication functions to secure the backend API. 
- API: [AWS Lambda](https://aws.amazon.com/lambda/), [Amazon API Gateway](https://aws.amazon.com/api-gateway/). JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway.
- Database: [Amazon DynamoDB](https://aws.amazon.com/dynamodb/). DynamoDB provides a  persistence layer where data can be stored by the API's Lambda function.


[Example repo](https://github.com/aws-samples/aws-serverless-workshops/tree/master/WebApplication)


## Multi Region Failover

This session talked about why serverless. how distribute traffic (DNS), Amazon API Gateway, DynamoDB (w/Global Tables), Cloud 9, AWS Lambda,

![Web Application Architecture](https://github.com/aws-samples/aws-serverless-workshops/blob/master/MultiRegion/images/architecture_new.png)

- The application must be able to failover to another region in the case of a disaster. The RTO and RPO must both be less than 15 minutes.
- Failover: Use Route53 to automatically use health check fail information and then point your domain at your secondary region.

[Example repo](https://github.com/aws-samples/aws-serverless-workshops/tree/master/MultiRegion)

## Microservices with Docker and AWS Fargate

![Monolith Architecture](https://github.com/aws-samples/aws-modern-application-workshop/blob/fargate/workshop-1/images/03-arch.png)

![Microservice using Fargate](https://github.com/aws-samples/aws-modern-application-workshop/blob/fargate/workshop-1/images/04-arch.png)

[Example repo](https://github.com/aws-samples/aws-modern-application-workshop/tree/fargate/workshop-1)

## Actions
Discuss with team about: 
1. How can we reduce deploy downtown? What would be the bottleneck to minimun downtown? 
2. Do we want to add multi region failover now? 
3. If we want to scale up to other region, can we do that automatically? How can we better use auto scale group
