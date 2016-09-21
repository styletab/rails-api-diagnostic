# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
// The purpose of a backend is to allow for persistance and storage of data. A
backend also allows for multiple users to interact with each other on an app. 
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
// Model
```

Which layer in the MVC pattern communicates with the model?

```bash
// Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
// Our client handles the responsibilities of the view.
```

What does C.R.U.D stand for?

```bash
// Create Read Update Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
// Controller
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
// Create, index, show, update, and destory
```

A user action fires a `GET` request for `/persons/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
// - Client sends the get request to to the server
- Server send the request to the router who sends to the controller asking for
- /persons/show/1
- Controller fires the show method to the Model
- The model communicates with the database to see if the parameters match (sql)
- If the data exists the database will return it to the model
- The model will return it to the controller
- The controller will return it to the Server
- The server will return the response to the client and the browser will render the
- proper view for the user.
```

What is the command to generate a new rails-api app?

```bash
// rails-api new [insert name sans brackets]
```

What is the command to start an instance of a rails server?

```bash
// bundle exec rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
// - create: bundle exec rake db:create
 - drop: bundle exec rake db:drop
 - migrate: bundle exec rake db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
// bundle exec rails-api g pets name:text age:integer
```
