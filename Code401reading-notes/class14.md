# Event Driven Architecture

**What’s the difference between a FIFO and a standard queue?**

- Standard queue tries to preserve the order of messages (best-effort), but there is a possibility of a message being delivered out of order.
- FIFO queue, messages are grouped into Message groups and all messages within a message group are sent and received in strict order.

**How can the server be assured a message was properly received?**

- By storing the messages at the message queue until the client is confirmed that the message was received, then delete it .

**What classic design pattern is best represented by event driven programming?**

1. Consume and Project: this pattern can help when you have a bottleneck legacy service that stores “popular” data of large domain objects.
2. Event-driven from end to end: the request-reply model is especially common in browser-server interactions.

**How do you test an event driven system?**

- Arrange — Setup prerequisites for the test.

- Act — Hit the trigger point to produce the event by microservice.

- Assert — Assert the event produced by microservice against the contract of its consumer.

## Terms

- FIFO Queue: FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated.

- Pub/Sub: Pub/Sub allows services to communicate asynchronously, with latencies on the order of 100 milliseconds, and enables you to create systems of event producers and consumers, called publishers and subscribers. Publishers communicate with subscribers asynchronously by broadcasting events, rather than by synchronous remote procedure calls (RPCs).

### SNS vs SQS Comparison

- SNS: Amazon Simple Notification Service (Amazon SNS) is a managed service that provides message delivery from publishers to subscribers (also known as producers and consumers). Publishers communicate asynchronously with subscribers by sending messages to a topic, which is a logical access point and communication channel. Clients can subscribe to the SNS topic and receive published messages using a supported endpoint type, such as Amazon Kinesis Data Firehose, Amazon SQS, AWS Lambda, HTTP, email, mobile push notifications, and mobile text messages (SMS).

- SQS: Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS eliminates the complexity and overhead associated with managing and operating message-oriented middleware, and empowers developers to focus on differentiating work. Using SQS, you can send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available.