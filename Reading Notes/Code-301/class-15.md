# Class 15

## [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

### What is OAuth?

    A secure, third-party, user-agent, delegated authorization framework

### Give an example of what using OAuth would look like

    When you want to log into an app and the app let's you log in with a 3rd party's authentication of your credentials 

### How does OAuth work? What are the steps that it takes to authenticate the user?

    1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    2. The second site generates a one-time token and a one-time secret unique 2.to the transaction and parties involved.
    3. The first site gives this token and secret to the initiating user’s client software.
    4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    6. The user approves (or their software silently approves) a particular transaction type at the first website.
    7. The user is given an approved access token (notice it’s no longer a request token).
    8. The user gives the approved access token to the first website.
    9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
    10. The second website lets the first website access their site on behalf of the user.
    11. The user sees a successfully completed transaction occurring.
    12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

### What is OpenID?

    For authentication. "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

## [Authorization and Authentication flows](https://auth0.com/docs/flows)

### What is the difference between authorization and authentication?

    Authentication is the process of a user/subject proving its ownership of a presented identity, by providing a password or some other uniquely owned or presented factor. Authorization is the process of letting a subject access resources after a successful authentication, oftentimes somewhere else.

### What is Authorization Code Flow?

    An authorization code passed through the server side and exchanged for a token

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    A way to mitigate the problems with authO handling single page web apps differently than mobile apps

### What is Implicit Flow with Form Post?

    A way for an app to let a user login without the need to hide or store client secrets

### What is Client Credentials Flow?

    Machine to machine authorization

### What is Device Authorization Flow?

    A way to ask the user to go to a link on their computer or smartphone in order to login 

### What is Resource Owner Password Flow?

    "Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used."

## Videos

Bookmark and Review

### [Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)
