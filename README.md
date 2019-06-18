# IDP Tempalte to setup a platform

## Feature


## Architectural Decisions & Options

<!-- adrlog -->

- [ADR-0001](0001-record-architecture-decisions.md) - Record architecture decisions
- [ADR-0002](0002-use-a-hosted-identity-solution-over-a-self-hosted-one.md) - Use a hosted Identity Solution over a self hosted one.
- [ADR-0003](0003-use-aws-cognito-as-idp-over-auth0-and-firbase-auth.md) - Use AWS Cognito as IDP over Auth0 and Firebase Auth

<!-- adrlogstop -->

## Setup

1. Understand the Concept of [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) / [Overview from AWS Summit](https://www.youtube.com/watch?v=jLQjQpUYw6g).
2. Configuration of new account -> [Docs](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-getting-started.html)
3. Setup a User Pool [Docs](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-as-user-directory.html)
4. Enable a hosted web ui [Docs](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-configuring-app-integration.html)
... implement your management/ app ui ...
5. Connect UI to cognito SSO either with Amplify or with Cognito SDK.
6. Add more platform information that is required like tenant id.