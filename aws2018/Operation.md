# Operation

## Management and Operations with AWS Fargate

### Goals
- Log Analysis with CloudWatch Logs and Elasticsearch
- Distributed Tracing and Debugging with AWS X-Ray
- Implementing Task Auto-Scaling

Scheduling and orchestration
Cluster Management, Placement Engine 

AWS Fargate take care of Availability Zones


- Amazon ECS Constructs
    - Observability
        - Monitoring
        - Logging
        - Tracing
        - Alerts
    - Monitoring
        - CloudWatch ECS Metrics 
        - ECS metadata endpoint
        - Partners: Datadog, dynatrace
    - Logging
        - CloudWatch Logging 
    - Distributed Tracing
        - X-Ray
    - Alerting
        - CloudWatch 
        - Service Integration
            - Amazon SNS
            - Amazon Lambda (event driven)

![Logging](/images/logging.JPG)

![ECS Constructs](/images/ECS_constructs.JPG)

![Stack](/images/stack.JPG)


[Example Repo](https://github.com/aws-samples/aws-modern-application-workshop/tree/fargate/workshop-3)


## Actions




