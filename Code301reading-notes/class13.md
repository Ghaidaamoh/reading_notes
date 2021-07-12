# Status Codes Based On REST Methods

- In your own words, describe what each group of status code represents:
  - 100’s = It's will telling the client that its request will fail before they start sending the body.
  - 200’s = It's means that these are the success codes,they tell the client that its request was accepted.
  - 300’s = It's means that these are redirection codes,they tell the client that the resource they are requesting isn’t available at the expected location anymore.
  - 400’s = It's means that these are the client error codes.
  - 500’s = It's means that these are the server error codes.

- What is a status code 202?
  - It's stauts is Accepted.

- What is a status code 308?
  - It's stauts is Permanent Redirect.

- What code would you use if an update didn’t return data to a client?
  - The 204 No Content .

- What code would you use if a resource used to exist but no longer does?
  - The 410 Gone.

- What is the ‘Forbidden’ status code?
  - 403 Forbidden : it's means the client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

- What is the difference beween PUT and PATCH?
  - patch : when we need to update based on what the user passes us put : it will update all the info to describe it all at once instead of the info that gets passed

- How do you make a defalut value in a schema?
  - so we are just going to use default and set this to date.now ,if we don’t pass our date it is just going to default it to current date