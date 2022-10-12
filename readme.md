# Test
We have made more tasks than you will realistically have time for. It is completely ok if you get stuck. Googling and asking questions is allowed.

The look of the website is not in scope, however the HTML structure should follow best practices.
We recognise that performing well in a situtation like this can be difficult. If you have to make some hacks to make something work, that's is completely ok. Just communicate your thoughts.

You do not have to solve the tasks in the order they are listed. Feel free to pick and choose.

## Api information
There is an api at <https://altinget-interview.azurewebsites.net/>. Documentation of API is at <https://altinget-interview.azurewebsites.net/swagger/index.html>.

For authentication there is a single user with the following credentials:

Username: `admin`

Password: `SuperSecret`

Some articles have a paywall. In this case they will not include the `articleText` unless an authorization token is supplied.

## Consume api

- List all articles, using the `Article` endpoint. Do not show the `articleText` in the list view.
- The `Article` endpoints sorts posts by the headline. Sort them by `id` instead.
- In the list of articles, diplay the create time in the following format: `dd-mm-yyyy`
- Make an article clickable so it leads to single article. If it has a paywall the user should see the paywall.
- List the 10 newest articles. Allow the user to fetch the next 10 articles. Infinite scrolling, view more, or pages, up to you.
- Use the `Article/search/{searchWord}` endpoint to allow the user to search for articles.
- Allow the user to search for content. There is no endpoint for this, so you'll have to implement it in the frontend.

## Auth

The API allows users to login with the `Login` endpoint. The returned token can be used in the Authorization header to create, update, and delete articles.

- Create a form allowing the user to login.
- When the user is logged in, they should be able to perform the following actions:
  - Read an article, including those behind a paywall.
  - Delete a post.
  - Edit a post.
  - Create a post.
