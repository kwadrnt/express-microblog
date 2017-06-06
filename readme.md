# <img src="https://cloud.githubusercontent.com/assets/7833470/10899314/63829980-8188-11e5-8cdd-4ded5bcb6e36.png" height="60"> Express Microblog

**Goal:** Use Node.js, Express, and MongoDB to build a full-stack microblog application.

## API Specifications

* Create a server with RESTful API endpoints for blog posts and comments. Your API should have the following five routes:
  * `GET /api/posts` to READ all blog posts
  * `POST /api/posts` to CREATE a new blog post
  * `GET /api/posts/:id` to READ one blog post
  * `POST /api/posts/:id/comments` to CREATE a comment on a particular post
  * `PUT /api/posts/:id` to UPDATE one blog post (bonus)
  * `DELETE /api/posts/:id` to DELETE one blog post (bonus)
  
* Set up a persistent database to store blog posts and comments. Blog posts and comments should have separate Mongoose schemas.  Blog posts should at minimum have a `title` and `description`. Comments should have `content`.

* Use AJAX and write client-side "templating" functions (with string template literals) to set up a website interface. Using this interface, **a user should be able to:**
  * See a list of all blog posts
  * Create a new blog post
  * Create a comment for a blog post
  * Delete an existing blog post (bonus)
  * Update an existing blog post (bonus)
  
* A pleasing a logical user experience in terms of user workflow

## Bonus

* Prevent invalid data from being saved into the database, and handle errors in your API routes.
* Add a User model and incorporate **local** authentication or one of the oauth **provider** strategies through [Passport.js](http://passportjs.org/docs).
* Build a "likes" functionality that lets users "upvote" blog posts.
* Add a "category" attribute to your blog posts. When a user clicks on a category, take them to a page that displays all the blog posts that have that category.

## Tips for Getting Started

1. Create a new directory for this project, and initialize a git repository in that directory. 
2. Add a README with a link to this page in case you want to reference it later, and make your first commit.
3. `npm init` to get your Node.js project started. You'll need to install the following node modules:
  * `express`
  * `body-parser`
  * `mongoose`
4. Use Postman or `curl` to test and debug your API routes. Make sure you are always `console.log`-ing data that comes back from your API when you make an AJAX call before you write any other code that relies on that data. 
5. Commit frequently.  When you are finished with this work for the morning, push your work to GitHub.
