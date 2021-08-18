# SQS and SNS

## Monolithic apps and microservices
- Apps are made of multiple components.
- The components communicate with each other to transmit data, fulfill requests, and keep the app running.
- Suppose that you have an app with tightly coupled components. These components might include databases, servers, the user interface, business logic, and so on => This architecture is a **monolithic application** 

=> **To help maintain application availability when a single component fails, you can design your application through a microservice approach**

- In a **microservice** approach, application components are loosely coupled. In this case, if a single component fails, the other component continue to work because they are communicating with each other. The loose coupling prevents the entire application from failing.
- When designing applications on AWS, you can take a microservice approach with services and components that fulfill different functions. Two services facilitate application integeration: **Amazon Simple Notification Service (Amazon SNS)** and **Amazon Simple Queue Service (Amazon SQS)**

## Amazon SNS - Amazon Simple Notification Service
- A publish/subscribe service. 
- Using SNS topics, a publisher publishes messages to subcriber. This is similar to the coffee shop: the cashier provides coffee orders to the barista who makes the drinks.
- In SNS subcribers can be web servers, email addresses, AWS Lambda functions, or several other options.

## Amazon SQS - Amazon Simple Queue Service
- A message queuing service
- You can send, store, and receive messages between software components without losing messages or requiring other services to be available.
- In SQS an application sends messages into a queue.
- A user or service retrieves a message from the queue, processes it and then deletes it from the queue.
- 