# Access Control (ACL)

**When is Basic Authorization used vs. Bearer Authorization?**

- The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret
- The Bearer authentication scheme is dedicated to the authentication using a token and is described

**What does the JSON Web Token package do?**

- JSON Web Token JWT is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

**What considerations should we make when creating and storing a SECRET?**

1. Never store unencrypted secrets in .git repositories
2. Don’t share your secrets unencrypted in messaging systems like slack
3. Store secrets safely
4. Restrict API access and permissions

## Terms

- encryption: Encryption is a way of scrambling data so that only authorized parties can understand the information. In technical terms, it is the process of converting human-readable plaintext to incomprehensible text, also known as ciphertext.

- token: equence of characters having a collective meaning. The character sequence forming a token is called the Lexeme.

- bearer: is an HTTP authentication scheme that involves security tokens called bearer tokens.

- secret: the secret is a symmetric key that is known by both the sender and the receiver.

- JSON Web Token: JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

### RBAC

**Role-Based Access Control RBAC**

- It is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

**What is RBAC?**

- It's idea of assigning system access to users based on their role within an organization.
- The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment.

**Benefits of RBAC?**

1. it is much easier to audit user rights, and to correct any issues identified.
2. easy to implement

**RBAC vs. ABAC vs. ACL**

- Access control lists ACL: is a means of defining access rights by a given user or user group, to a specific object, such as a document.
- Attribute-based access control ABAC:sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access,...