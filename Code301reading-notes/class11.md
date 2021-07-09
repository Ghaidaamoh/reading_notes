
# What is OAuth

- TWhat is OAuth?
  - OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

- Give an example of what using OAuth would look like.
  - When you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.

**How does OAuth work? What are the steps that it takes to authenticate the user?**

1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider.
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After   authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves a particular transaction type at the first website.
7. The user is given an approved access token.
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.

- What is OpenID?

  - It's allows you to use an existing account to sign in to multiple websites, without needing to create new passwords.

  
## Authorization and Authentication flows

- What is the difference between authorization and authentication?
   - Authentication confirms that users are who they say they are. Authorization gives those users permission to access a resource.

- What is Authorization Code Flow?
   - It's is used to obtain an access token to authorize API requests. And the Access tokens, obtained using authorization code flow, provide permissions for your application to manipulate documents and other resources on behalf of a Mendeley user and make requests for all API resources.

- What is Authorization Code Flow with Proof Key for Code Exchange PKCE?
   - The Authorization Code Flow PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users.

- What is Implicit Flow with Form Post?
   - It's means that the web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

- What is Client Credentials Flow?
   - The Client Credentials flow is a server to server flow. There is no user authentication involved in the process.

- What is Device Authorization Flow?
   - It's an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token.

- What is Resource Owner Password Flow?
   - It's a requests that users provide credentials username and password, typically using an interactive form.

