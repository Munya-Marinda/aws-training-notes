# Module 2: Applications in the Cloud

## Topic A: Availability

- **Elastic Load Balancer**: Ensures the availability of Application servers.
- **Database Availability**: In case the primary DB fails, a secondary database can be automatically cloned with a click of a button, and the secondary database will take over.

## Topic B: Messaging Services

- Transition to Microservices from Monolithic Applications.
- **Amazon SNS (Simple Notification Service)**

  - Amazon SNS is a pub/sub messaging service designed to decouple microservices, distributed systems, and serverless applications. It offers the flexibility to send messages to various endpoints, including email addresses, mobile phone numbers, and HTTP endpoints.
  - Versatile Functionality: Amazon SNS does a lot, including sending SMS, emails, and more. It can be used for both Application-to-Person and Application-to-Application messaging.

- **Amazon SQS (Simple Queue Service)**
  - Amazon SQS is the preferred choice when it comes to processing messages one by one.
  - Examples of Use:
    - Imagine a restaurant chef preparing meals according to incoming orders, one at a time.
    - Buffer and Batch Operations: SQS excels at buffering and batching operations. It can improve application performance by reducing the number of requests made to other services. For instance, SQS can buffer requests to a database until the queue reaches a certain size, allowing the application to process multiple requests in one go.

## Topic C: Serverless Compute Services

- **AWS Lambda**
  - Lambda is an event-driven service that simplifies serverless computing.
  - How it Works:
    1. Upload Code: You upload your code to Lambda.
    2. Set Triggers: Define events that will trigger the Lambda function.
    3. Event-Driven Execution: Lambda automatically executes your code when the specified events occur.

**Interactive Demo: Using Lambda Functions**
