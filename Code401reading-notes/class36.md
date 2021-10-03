# Application State with Redux

**What are the advantages of storing tokens in “Cookies” vs “Local Storage”**

- Local Storage

  - Pros: It's convenient.

  - It's pure JavaScript and it's convenient. If you don't have a back-end and you're relying on a third-party API, you can't always ask them to set a specific cookie for your site. Works with APIs that require you to put your access token in the header like this: Authorization Bearer ${access_token}.

- Cons: It's vulnerable to XSS attacks.

  - An XSS attack happens when an attacker can run JavaScript on your website. This means that the attacker can just take the access token that you stored in your localStorage.

- Cookies

  - Pros: The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.

  - Cons: Depending on the use case, you might not be able to store your tokens in the cookies.

    - Cookies have a size limit of 4KB. Therefore, if you're using a big JWT Token, storing in the cookie is not an option.

**Explain 3rd party cookies.**

- Third-party cookies are created by domains that are not the website (or domain) that you are visiting. These are usually used for online-advertising purposes and placed on a website through adding scripts or tags. A third-party cookie is accessible on any website that loads the third-party server’s code.

**How do pixel tags work?**

- It’s a 1×1-pixel graphic used for tracking user behavior, site conversions, web traffic, and other metrics at a site’s server level. In other words, it is a tiny pixel-sized image, usually hidden, embedded in everything, from banner ads to emails.

## Terms

- cookies: Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

- authorization: Authorization is the process of giving someone the ability to access a resource.

- access control: Access control is a security technique that regulates who or what can view or use resources in a computing environment. It is a fundamental concept in security that minimizes risk to the business or organization.

- conditional rendering: Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition. This concept is applied often in the following scenarios:

  - Rendering external data from an API.
  - Showing or hiding elements.
  - Toggling application functionality.
  - Implementing permission levels.
  - Handling authentication and authorization.
