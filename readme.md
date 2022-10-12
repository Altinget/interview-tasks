# Test

There is an api at <https://altinget-interview.azurewebsites.net/>. Documentation of API is at <https://altinget-interview.azurewebsites.net/swagger/index.html>.

We have made more tasks than you will realistically have time for. It is completely ok if you get stuck. Googling and asking questions is allowed. We will pay attention to:

- Code quality
- Your thoughts and considerations
- Error handling
- Security

The design of the website is not in scope, however the HTML structure should follow best practices.
We recognise that performing well in a situtation like this can be difficult. If you have to make some ugly code to make something work, that's is completely ok. Just communicate your thoughts.

You do not have to solve the tasks in the order they are listed. Feel free to pick and choose.

## Consume api

- List all articles, using the `Article` endpoint.
- In the list of articles, diplay the create time in the following format: `dd-mm-yyyy`
- Make an article clickable so it leads to single article.
- List the 10 newest articles. Allow the user to fetch the next 10 articles. Infinite scrolling, view more, or pages, up to you.
- Use the `Article/search/{searchWord}` endpoint to allow the user to search for articles.
- Allow the user to search for content. There is no endpoint for this, so you'll have to implement it in the frontend.
- The `Article` endpoints sorts posts by the headline. Sort them by `createTime` instead.

## Auth

The API allows users to login with the `Login` endpoint. The returned token can be used in the Authorization header to create, update, and delete articles.

There is a single user with the following credentials:

Username: `admin`

Password: `SuperSecret`

- Create a form allowing the user to login.
- When the user is logged in, they should be able to perform the following actions:
  - Delete a post.
  - Edit a post.
  - Create a post.
