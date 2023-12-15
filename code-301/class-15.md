# Authentication

OAuth (Open Authorization):

OAuth is an open standard for access delegation, commonly used as a way for users to grant third-party applications limited access to their resources without sharing their credentials. It is often used to enable secure authorization and access to APIs (Application Programming Interfaces) on behalf of a user.

Example of OAuth Flow:

Let's consider an example where you want to allow a third-party application to access your Google Calendar on your behalf:

User Initiates Authorization:

You decide to connect a third-party calendar application to your Google Calendar.
The third-party application requests permission to access your Google Calendar.
Redirect to Authorization Server:

The third-party application redirects you to Google's OAuth server.
This redirection includes information such as the scope of access requested and the callback URL.
User Grants Permission:

At Google's OAuth server, you log in (if not already) and are presented with a consent screen that outlines the requested permissions.
You grant permission to the third-party application.
Authorization Server Issues Access Token:

Google's OAuth server issues an access token to the third-party application.
Third-party Application Accesses API:

The third-party application uses the received access token to access your Google Calendar on your behalf.
Access Token Usage:

The access token acts as a temporary, revocable key that allows the third-party application to access specific resources on the user's behalf.
OAuth Workflow Steps:

Client Registration:

The third-party application (client) registers with the OAuth server, obtaining a client ID and client secret.
Authorization Request:

The client initiates the authorization process by redirecting the user to the authorization server. This includes the client ID, scope, and redirect URI.
User Authorization:

The user interacts with the authorization server, granting or denying permission.
Access Token Request:

If the user grants permission, the authorization server issues an access token to the client.
Access Token Usage:

The client uses the access token to access protected resources on the resource server (API).
OpenID:

OpenID is a related authentication protocol that complements OAuth. While OAuth is primarily focused on authorization, OpenID provides a standard for user authentication. OpenID allows users to use a single set of credentials to log in to multiple services without the need to create separate usernames and passwords for each.

Authorization Code Flow:

Description: The most secure and commonly used flow. The client obtains an authorization code, exchanges it for an access token, and then uses the access token to access resources.
Authorization Code Flow with Proof Key for Code Exchange (PKCE):

Description: Enhances the security of the Authorization Code Flow by adding a dynamic secret (code verifier), protecting against authorization code interception.
Implicit Flow with Form Post:

Description: Deprecated due to security concerns. The access token is obtained directly as part of the redirect URL, which may expose sensitive information.
Client Credentials Flow:

Description: Used by confidential clients (e.g., server-to-server communication) to obtain an access token by presenting the client's credentials (client ID and secret).
Device Authorization Flow:

Description: Designed for devices with limited input capabilities (e.g., smart TVs). The user authorizes the device through a secondary device, and the client polls to obtain the access token.
Resource Owner Password Flow:

Description: Deprecated due to security risks. The user provides their username and password directly to the client, which exchanges them for an access token.
Key Characteristics:

Authorization Code Flow:

Use Case: Web applications with server-side code.
Security: Higher security due to server-side token exchange.
Authorization Code Flow with PKCE:

Use Case: Mobile and Single Page Applications (SPAs) with a client-side code.
Security: Improved security for SPAs, mitigating authorization code interception.
Implicit Flow with Form Post:

Use Case: Deprecated, not recommended for use.
Security: Lower security due to exposing tokens in the URL.
Client Credentials Flow:

Use Case: Server-to-server communication.
Security: Suitable for confidential clients.
Device Authorization Flow:

Use Case: Devices with limited input capabilities.
Security: Provides a secure method for device authorization.
Resource Owner Password Flow:

Use Case: Deprecated, not recommended for use.
Security: Lower security due to exposing the user's credentials to the client.

Videos
Bookmark and Review
Auth0 for single page apps

## Things I want to know more about