# AWS: Events

**Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

- Amazon API Gateway is an AWS service for creating, publishing, maintaining, monitoring, and securing REST, HTTP, and WebSocket APIs at any scale. API developers can create APIs that access AWS or other web services, as well as data stored in the AWS Cloud.
- Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

**List the AWS Database offerings and talk about the pros and cons of each**

1. Relational: Traditional applications, ERP, CRM, e-commerce
   - Amazon Aurora
   - Amazon Relational Database Service (RDS)
   - Amazon Redshift
2. Key-value: High-traffic web apps, e-commerce systems, gaming applications
   - Amazon DynamoDB
3. In-memory: Caching, session management, gaming leaderboards, geospatial applications
   - Amazon ElastiCache for Memcached
   - Amazon ElastiCache for Redis
   - Amazon MemoryDB for Redis
4. Document: Content management, catalogs, user profiles
   - Amazon DocumentDB (with MongoDB compatibility)

**Pros and Cons:**

1. Availability on several database instances

2. Six familiar database to chose from

3. Efficient

4. Scalable

5. Cost reduction

6. Resizable capacity

7. Automating time consuming administration tasks

8. No root access to server.

9. Downtime required

10. Not a zero administration database.

11. Read Shreya Sh

**What’s the difference between a FIFO and a standard queue?**

- Message Order

  - Standard queues provide best-effort ordering which ensures that messages are generally delivered in the same order as they are sent.
  - FIFO queues offer first-in-first-out delivery and exactly-once processing: the order in which messages are sent and received is strictly preserved

- Delivery

  - Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue
  - FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue

**How can the server be assured a message was properly received?**

- By storing the messages at the message queue until the client is confirmed that the message was received, then delete it .

## Terms

- Serverless API: is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

- Triggers: is a set of Structured statements that automatically fires off an action when a specific operation, such as changing data in a table, occurs. A trigger consists of an event an INSERT, DELETE, or UPDATE statement issued against an associated table and an action .

- Dynamo vs Mongo:

1. MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
2. DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
3. DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
4. DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
5. DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.

### SNS vs SQS Comparison

- SNS: Amazon Simple Notification Service (Amazon SNS) is a managed service that provides message delivery from publishers to subscribers (also known as producers and consumers). Publishers communicate asynchronously with subscribers by sending messages to a topic, which is a logical access point and communication channel. Clients can subscribe to the SNS topic and receive published messages using a supported endpoint type, such as Amazon Kinesis Data Firehose, Amazon SQS, AWS Lambda, HTTP, email, mobile push notifications, and mobile text messages (SMS).

- SQS: Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS eliminates the complexity and overhead associated with managing and operating message-oriented middleware, and empowers developers to focus on differentiating work. Using SQS, you can send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available.