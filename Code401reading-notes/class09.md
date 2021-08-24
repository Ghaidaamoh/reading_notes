# Authorization/Authentication

**What header(s) are used in authentication and authorization**

1. Basic Auth: Authorization header that contains the word Basic, followed by a space and a base64-encoded(non-encrypted) string username: password.

- Authorization: Basic AXVubzpwQDU1dzByYM==
- Base64 encoding does not mean encryption or hashing!

2. Bearer Token: Bearer Authentication gives access to the bearer of this token.

- Authorization: Bearer

3. API Key: API key auth, you send a key-value pair to the API either in the request headers or query parameters.

- GET /endpoint?api_key=abcdefgh123456789

4. Digest Auth:Digest Authentication communicates credentials in an encrypted form by applying a hash algorithm to the username and the password, the password is converted to response and then it is sent to the server.

- Authorization: Digest username=”admin” Realm=”abcxyz” nonce=”474754847743646”, uri=”/uri” response=”7cffhfr54685gnnfgerg8”

**Digest Auth steps:**

- Client sends a request to the server
- The server responds with a special code called a nonce i.e. number used only once, another string representing the realm a hash for authentication from the client.
- The client responds with this nonce and an encrypted version of the username, password, and realm a hash
- If the Client hash matches the server hash, the server will respond with the requested information. Otherwise, it will pass an error message.

5. OAuth 2.0: you first retrieve an access token for the API, then use that token to authenticate future requests.

- Authorization: Bearer hY_9.B5f-4.1BfE //where “hY_9.B5f-4.1BfE” is your OAuth Access Token

**An OAuth 2.0 flow works as follows:**

- A client application makes a request for the user to authorize access to their data.
- the user grants access, the application then requests an access token from the service provider, passing the access grant from the user and authentication details to identify the client.
- The service provider validates these details and returns an access token.
- The client uses the access token to request the user data via the service provider.

6. Hawk Authentication: Hawk authentication enables you to authorize requests using partial cryptographic verification.

- Authorization: Hawk id="abcxyz123", ts="1592459563", nonce="gWqbkw", mac="vxBCccCutXGV30gwEDKu1NDXSeqwfq7Z0sg/HP1HjOU="

**The Hawk Authentication parameters are as follows:**

- Hawk Auth ID: Your API authentication ID value.
- Hawk Auth Key: Your API authentication key value.
- Algorithm: The hash algorithmsha266,sha1 used to create the message authentication codeMAC.

7.  AWS Signature: AWS is the authorization workflow for Amazon Web Services requests. AWS uses a custom HTTP scheme based on a keyed-HMAC Hash Message Authentication Code for authentication.

- Authorization: AWS4-HMAC-SHA256 Credential=abc/20200618/us-east-1/execute-api/aws4_request, SignedHeaders=host;x-amz-date, Signature=c6c85d0eb7b56076609570f4dbdf730d0a017208d964c615253924149ce65de5

**The AWS Authentication parameters are as follows:**

- Access Key: API Access key value.
- Secret Key: API Secret key value.

## What is safe to put into a JWT

1. Registered Claims:

- subject: identifies the principal that is the subject of the JWT. Must be unique
- expiration time: identifies the expiration time after which you must no longer accept this token.

2. Public claims:

- with public names or names registered which contain values that should be unique like email, address or phone_number

3. Private claims to use in your own context and values can collision

**How are JWTs validate**

- the server validates the username and password combination and creates a JWT token with a payload containing the user technical identifier and an expiration timestamp.

### Terms

- RBAC:Role-based access control RBAC restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

- User Roles: are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.

- JWT Token: JSON Web Token JWT is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.