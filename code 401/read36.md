## Amplify and Cognito
- Amplify Auth provides an interface for authentiating a user.
- simple api to check the current auth session.
- execute `amplify add auth` to start provisioning auth resources in the backend, follow the prompts then `amplify push`. should update `amplifyconfiguration.json`
- add dependencies
- add plugins
- intial test from MainActivity's `onCreate` method
- register a user
- confirmation code will be sent to the email id provided during sign up.
- can enable guest access if desired
