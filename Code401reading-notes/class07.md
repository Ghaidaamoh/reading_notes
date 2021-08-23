# Bearer Authorization

**Write the following steps in the correct order:**

- Receive access token
- Redirect to a third party authentication endpoint
- Register your application to get a client_id and client_secret
- Make a request to a third-party API endpoint
- Ask the client if they want to sign in via a third party
- Receive authorization code
- Make a request to the access token endpoint

**Correct Order:**

1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Redirect to a third party authentication endpoint
4. Make a request to a third-party API endpoint
5. Receive authorization code
6. Make a request to the access token endpoint
7. Receive access token

**What can you do with an authorization code?**

- It's is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.

**What can you do with an access token?**

- Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data.
Access tokens must be kept confidential in transit and in storage.

**What’s a benefit of using OAuth instead of your own basic authentication?**

- It enables apps to obtain limited access (scopes) to a user’s data without giving away a user’s password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities. It supports server-to-server apps, browser-based apps, mobile/native apps, and consoles/TVs.

## JWT

**What is JSON Web Token?**

- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

**When should you use JSON Web Tokens?**

1. Authorization:
2. Information Exchange:

**What is the JSON Web Token structure?**

1. Header
2. Payload
3. Signature

- Therefore, a JWT typically looks like the following.
   - xxxxx.yyyyy.zzzzz

**Why should we use JSON Web Tokens?**

- Security-wise, SWT can only be symmetrically signed by a shared secret using the HMAC algorithm.