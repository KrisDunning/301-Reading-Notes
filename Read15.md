[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----

# Reading 15 - Authentication

## Reading - What is OAuth

> What is OAuth?

- An open-standard authorization protocol(1.0) or framework(2.0) that facilitates single sign on solutions across the web.

> Give an example of what using OAuth would look like.

- When you are able to use facebook or google to sign into another website just by clicking a "use my google account" button to log in.

> How does OAuth work? What are the steps that it takes to authenticate the user?

- 1.) website 1 connects to website 2 on behalf of the user.
- 2.) webstie 2 generates a one-time token and a one-time secret unique to the transaction.
- 3.) website 1 give this token and secret to the users client.
- 4.) Client presents the request token and secret to their authorization provider(may or may not be website 2)
- 5.) Client may be asked to authenticate. After authentication the client is asked to approve the authorization transaction to website 2. 
- 6.) User or client approves a transaction at website 1.
- 7.) User is given an approved access token.
- 8.) The user gives the approved access token to website 1.
- 9.) website 1 gives the access token to website 2 as proof of authentication on behalf of user.
- 10.) website 2 lets website 1 access their site on behalf of user. 
- 11.) User sees a successfully completed transaction occurring.

> What is OpenID?

- It is the authentication layer for OAuth since 2014 when it was rebranded as OpenID Connect.

## Authorization and Authentication Flows

> What is the difference between authorization and authentication?

- Authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.

> What is Authorization Code Flow?

- Where a server side app exchanges an authorization code (and a client secret) for a token.

> What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

- For native and single-page applications due to additional security concerns. Includes a Proof Key. 

> What is Implicit Flow with Form Post?

- Implicit Flow is used for public clients or apps which are unable to securely store client secrets. When used with Form Post response is offers streamlined workflow if app only needs an ID token to perform user authentication.

> What is Client Credentials Flow?

- Machine to Machine apps dont use Username/Passwords so they use their client ID and client secret to authenticate themselves and get a token.

> What is Device Authorization Flow?

- Input limited devices ask the user to use a link or smartphone to authorize the device. For use with mobile/native apps. 

> What is Resource Owner Password Flow?

- When highly-trusted apps can request the users credentials (username/password), typically with an interactive form. Not generally reccommended.


## Things I want to know more about

When to use what? Is the basic flows okay for simple project websites?

-----
