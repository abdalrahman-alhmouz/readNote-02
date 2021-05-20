## Amplify and Cognito
- The Amplify Auth category provides an interface for authenticating a user. Behind the scenes, it provides the necessary authorization to the other Amplify categories.
- The Amplify CLI helps you to create and configure the auth category with an authentication provider.
- execute command `amplify add auth`
- push changes `amplify push`
- install dependencies
- check the current aith session. for testing run this from your MainActivity `onCreate` method
```
Amplify.Auth.fetchAuthSession(
        result -> Log.i("AmplifyQuickstart", result.toString()),
        error -> Log.e("AmplifyQuickstart", error.toString())
);
```
- register a user, confirm attributes like email/phone, and sign in with optional multi-factor authentication.
- confirmation code will be sent to the email id
- The AWS Cognito Auth Plugin can be configured to automatically obtain guest credentials once the device is online so that you are able to use other categories “anonymously” without the need to sign in.
