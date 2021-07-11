# Read11: Authentication


## What is OAuth
- What is OAuth?

 _"is anopen-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential"_*

- Give an example of what using OAuth would look like.

Using one email account to log into another website, without entering a user or a password. the email account (third party) will be responsible of giving you the permission.

- How does OAuth work? What are the steps that it takes to authenticate the user?

1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.

_steps are frem *_

- What is OpenID?

An authentication service. gives the user a single ID that allows him to login different websites using the same account. 


# Authorization and Authentication flows
- What is the difference between authorization and authentication?

authentication is the process of proving that the login is valid, proving it is unique. authorization is giving a third-party a limited permission to grant access to the user.

- What is Authorization Code Flow?

it exchanges an Authorization Code for a token.

- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

an additional security method, for Authorization Code Flow.

- What is Implicit Flow with Form Post?

solves the problem for Public Clients, or applications which are unable to securely store Client Secrets

- What is Client Credentials Flow?

instead of using a user ID and a password, Client Credentials Flow passes along their Client ID and Client Secret to authenticate themselves and get a token.


- What is Device Authorization Flow?

rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device


*definition from https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html 


