## Intro to Serverless
- Cloud computing execution model where cloud porvider dynamically manages the allocation and provisioning of servers.
- Price is based on the number of executions
- event-driven cloud-based system where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls (Functions as a Service)
- Serverless is reduced cost
- downside serverless functions are accessed only as private APIs. You can't access them through the usual IP
- For simple applications with few dependencies, Serverless is the winner; for anything more complex, Traditional Architecture is the winner.
- serverless app: A Serverless solution consists of a web server, Lambda functions (FaaS), security token service (STS), user authentication and database.

## AWS Ampify
- configure backends fast
- easily connect to your app
-deploy web apps in three steps
- AWS Amplify is an end-to-end solution that enables mobile and front-end web developers to build and deploy secure, scalable full stack applications, powered by AWS. With Amplify, you can configure app backends in minutes, connect them to your app in just a few lines of code, and deploy static web apps in three steps. Get to market faster with AWS Amplify

## GraphQL
- The GraphQL Transform provides a simple to use abstraction that helps you quickly create backends for your web and mobile applications on AWS. With the GraphQL Transform, you define your application’s data model using the GraphQL Schema Definition Language (SDL) and the library handles converting your SDL definition into a set of fully descriptive AWS CloudFormation templates that implement your data model.

- Object types that are annotated with `@model` are top-level entities in the generated API. Objects annotated with `@model` are stored in Amazon DynamoDB and are capable of being protected via `@auth`, related to other objects via `@connection`, and streamed into Amazon Elasticsearch via `@searchable`. You may also apply the `@versioned` directive to instantly add a version field and conflict detection to a model type.
