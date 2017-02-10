# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The purpose of a backend is to manage databases for your app, to see how many
users there are, and manage what they can do with your app.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The layer in the MVC that is used by the controller to fetch data is the model.
```

Which layer in the MVC pattern communicates with the model?

```md
The layer in the MVC that communicates with the model is the controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
We don't use views in our interpretation of the MVC pattern because we lump view
in with the controller.
```

What does C.R.U.D stand for?

```md
Create.
Read.
Update.
Delete.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
We would find the C.R.U.D actions in the controller part of the MVC because the
controller receives the HTTP request from the router.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
CREATE: `::create`,
READ: `::index, ::show`,
UPDATE: `::update`,
DELETE: `::destroy`.
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
-User makes an HTTP request using the verb `GET` (desires one person).
-Request gets sent to the router.
-Router sends it to the controller.
-Controller sends that to the model.
-Model accesses the database.
-Model finds info in database.
-Model "hands" it to the controller.
-Controller sends the response back to the user.
-User receives the response.
```

What is the command to generate a new rails-api app?

```bash
bundle install
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
-db:drop
-db:create
-db:migrate
-db:seed
-db:nuke_pave
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate model pet name:string age:integer
```
