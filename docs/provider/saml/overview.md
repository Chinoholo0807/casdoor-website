---
title: Overview
description: Using identities from external identity providers that support SAML 2.0
keywords: [SAML, Keycloak, Aliyun IDaas]
authors: [seriouszyx]
---

Casdoor can be configured to support user login to UI using identities from external identity providers that support SAML 2.0. In such a configuration, Casdoor can never store any credentials for the users.

Now, Casdoor supports many SAML application providers. Icons of providers will be shown in login page after adding to Casdoor. Here are the providers Casdoor supports:

|Aliyun IDaaS|Keycloak|
| :--: | :--: |
|<img src="https://cdn.casbin.org/img/social_aliyun.png" width="40"></img>|<img src="https://cdn.casbin.org/img/social_keycloak.png" width="40"></img>|
|✅|✅|

## Terms

- Identity Provider (IDP) - The service that stores the identity database and provides identity and authentication services to Casdoor.
- Service Provider (SP) - The service providing resources to the end user, in this case, the Casdoor deployment.
- Assertion Consumer Service (ACS) - The consumer of SAML assertions generated by the Identity Provider.

## How SAML integration works

When using SAML SSO, users log into the Casdoor via the identity provider without ever passing credentials to Casdoor. The progress is shown in the following diagram.

![SAML](/img/providers/SAML/SAML.png)
