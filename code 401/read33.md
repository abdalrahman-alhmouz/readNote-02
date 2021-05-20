## Serverless
- Serverless architecture is certainly very exciting, but it comes with a bunch of limitations. As the validity and success of architectures depend on the business requirements and by no means solely on technology. In the same way, Serverless can shine when used in proper place.

## AWS Amplify
- AWS Amplify is an end-to-end solution that enables mobile and front-end web developers to build and deploy secure, scalable full stack applications, powered by AWS. With Amplify, you can configure app backends in minutes, connect them to your app in just a few lines of code, and deploy static web apps in three steps. Get to market faster with AWS Amplify.
 - configure backends fast, easily connect, deploy in 3 steps

## GraphQL
- `@connection` enables your to spwcify relationships between `@model` types
- The fields argument can be provided and indicates which fields can be queried by to get connected objects. The keyName argument can optionally be used to specify the name of secondary index (an index that was set up using @key) that should be queried from the other type in the relationship.
- When specifying a keyName, the fields argument should be provided to indicate which field(s) will be used to get connected objects. If keyName is not provided, then @connection queries the target table’s primary index.
- Has One: can only reference the primary index of a model
-Has many: needs a `@key` that allows comments to be queried by the postID and the connection uses this key to get all comments whose postID is the id of the post was called on.
- Belongs to: bi-directional connection by adding a many to one connection to types that already have a one to many connection
- Many to many: two `@key` calls are needed on the PostEditor model. first create a Post and User and then add a connection between themwith by creating a PostEditor object 
