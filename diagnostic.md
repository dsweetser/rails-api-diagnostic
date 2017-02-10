# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
to store information beyond an single browser session and to allow for multiple
users to interact.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Views simply display what they're told to by the controller and thus are less
important to talk about in the chain.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The Controller translates the commands for the C.R.U.D. actions and the model
sends them to the server.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index, show, create, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
Request gets sent to the Router, which determines the controller to send it to
The Controller then sends it to the Model
The model sends a request to the database(db) for the information
The db sends the Model back the information
the controller receives that information and sense a response back to the client
```

What is the command to generate a new rails-api app?

```bash
rails new
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
ISSUE: should this not be 4 points?
bin/rails db:drop
bin/rails db:create
bin/rails db:migrate
bin/rails db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
