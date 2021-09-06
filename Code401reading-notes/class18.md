# AWS: S3 and Lambda

**What are serverless functions?**

- It's is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

**If you were to create a system that emulated Lambda functions, how would you do it?**

- To create a Lambda function with the console
  - Open the Functions page on the Lambda console.
  - Choose Create function.
  - Under Basic information, do the following:
     - For Function name, enter my-function.
     - For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET.

**Choose Create function.**

- Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources.

**Describe how a CDN works**

- A content delivery network (CDN) is a group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are.

- The mission of a CDN is to reduce latency. Latency is that annoying delay you experience when trying to access a web page or video stream before it fully loads on your device. Some content delivery networks alleviate latency by reducing the physical distance that the content needs to travel to reach you. Therefore, larger, more widely distributed CDNs are able to deliver web content more quickly and reliably by putting the content as close to the end user as possible.

## Terms

- Serverless Functions: serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies.
- Cloud Storage: Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service.
- CDN: A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content.

### AWS API Gateway

- It is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the front door for applications to access data, business logic, or functionality from your backend services.

**API Types**

1. RESTful APIs: build RESTful APIs optimized for serverless workloads and HTTP backends using HTTP APIs.

2. WEBSOCKET APIs: build real-time two-way communication applications, such as chat apps and streaming dashboards, with WebSocket APIs. API Gateway maintains a persistent connection to handle message transfer between your backend service and your clients.

**AWS DynamoDB Guide**

**What is DynamoDB?**

- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:
  - reliable performance even as it scales;
  - a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
  - a small, simple API allowing for simple key-value access as well as more advanced query patterns.
- DynamoDB is a particularly good fit for the following use cases:

   - Applications with large amounts of data and strict latency requirements.
   - Serverless applications using AWS Lambda. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.
   - Data sets with simple, known access patterns.

**AWS DynamoDB**

- Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale.
- It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.

**Dynamoose**

- Dynamoose is a modeling tool for Amazon's DynamoDB.
- Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

**Key Features**
- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling validation, required attributes, and more
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support