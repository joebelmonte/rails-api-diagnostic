# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
Without one it would not be possible for 2 (or more) people to access the same web app and
interact with each other.
It would also not be possible to save state and come back to the app later.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
It uses the model.
```

Which layer in the MVC pattern communicates with the model?

```md
Controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Serializers are a class that we use instead of the view.  It’s choosing which part of the object and in what format to send back.
```

What does C.R.U.D stand for?

```md
Create READ UPDATE DESTROY
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The model.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Get 1 --> Read
Get index/all --> Read
Post --> Create
Patch --> Update
Delete --> Destroy

```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. Find the appropriate Route, which tells you the controller and method to use
2. Go to the appropriate controller
3. Within the controller, fire the method
3. Method gets data from the model
4. Model send the data back to the method
5. Method returns the appropriate data in JSON or an error message.
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
bin/rake [db:drop] db:create db:migrate db:seed db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold post name:string age:integer user:references
```
